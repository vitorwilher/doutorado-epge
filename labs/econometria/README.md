# Laboratórios de Econometria em R

Revisão computacional das aulas da disciplina de Econometria do
MPEF/FGV-EPGE (Prof. Marcelo Mello). Cada notebook reproduz em R os resultados
centrais de uma aula.

Abrem no **Google Colab** com um clique — rodam no navegador, sem instalar nada.
O runtime é o de R; `ggplot2` e `dplyr` já vêm no Colab e a primeira célula
instala o que faltar.

| # | Aula | O que se vê rodando | |
|---|------|---------------------|---|
| 1 | Causalidade | Por que a aleatorização funciona; o viés da autosseleção; o *proxy* ruidoso | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vitorwilher/doutorado-epge/blob/main/labs/econometria/01-causalidade.ipynb) |
| 2 | Probabilidade | Binomial, Chebyshev, lei das expectativas iteradas, covariância zero sem independência | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vitorwilher/doutorado-epge/blob/main/labs/econometria/02-probabilidade.ipynb) |
| 3 | Regressão simples | MQO na mão contra `lm()`, ortogonalidade, TSS = ESS + SSR, distribuição amostral | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vitorwilher/doutorado-epge/blob/main/labs/econometria/03-regressao-simples.ipynb) |
| 4 | Inferência | Erro-padrão robusto do zero, cobertura do IC, heterocedasticidade, *dummy* = diferença de médias | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vitorwilher/doutorado-epge/blob/main/labs/econometria/04-inferencia.ipynb) |
| 5 | Regressão múltipla | Viés de variável omitida; ele **não** some com *n*; R² vs. R² ajustado; multicolinearidade | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vitorwilher/doutorado-epge/blob/main/labs/econometria/05-regressao-multipla.ipynb) |
| 6 | Teste F | Estatística de Wald do zero, F = t², o F homocedástico rejeitando 15% quando promete 5% | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vitorwilher/doutorado-epge/blob/main/labs/econometria/06-teste-f.ipynb) |
| 9 | Dados em painel | Efeitos fixos de estado e de tempo; *mais armas, menos crime* com dados reais; *within* = LSDV; erros-padrão clusterizados | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vitorwilher/doutorado-epge/blob/main/labs/econometria/07-dados-painel.ipynb) |

O **[índice comentado](https://colab.research.google.com/github/vitorwilher/doutorado-epge/blob/main/labs/econometria/00-indice.ipynb)** dá o panorama da sequência.

## Sobre os dados

Os exemplos de *TestScore* × *STR* (laboratórios 1 a 6) usam dados **simulados e
calibrados** para se parecerem com os de Stock & Watson (2020) — não são os dados
originais da Califórnia. É deliberado: numa simulação **conhecemos** os parâmetros
verdadeiros, e é isso que permite falar em viés com precisão em vez de por analogia.

O laboratório 9, em contrapartida, usa o painel ***Guns*** **real** — 51 estados
americanos de 1977 a 1999 —, baixado da web pelo próprio notebook.

## Rodar localmente

```bash
jupyter notebook          # requer o kernel IRkernel
```

ou extraindo o código de um notebook para um `.R` e rodando com `Rscript`.
Os laboratórios 1 a 6 não dependem de arquivos externos nem de rede; o 9 baixa o painel
*Guns* de uma fonte pública.

## Apostila

A apostila completa da disciplina (216 páginas, com derivações, as listas oficiais e
os gabaritos) está em
<https://vitorwilher.github.io/doutorado-epge/econometria/>.
