# Notas do Doutorado em Economia · EPGE/FGV

Site que reúne as **notas de aula do Doutorado em Economia**
da **EPGE/FGV**, disciplina a disciplina, com apostila própria para cada uma.
O acervo cresce a cada disciplina cursada ao longo do doutorado.

- **Autor das notas:** Vítor Wilher
- **Site:** publicado via GitHub Pages a partir da pasta [`docs/`](docs/)

| # | Disciplina | Professor(a) | Apostila |
|---|------------|--------------|----------|
| 1 | Matemática | Silvia Matos | [`docs/matematica/apostila.pdf`](docs/matematica/apostila.pdf) |
| 2 | Macroeconomia | Fernando de Holanda Barbosa Filho | [`docs/macroeconomia/apostila.pdf`](docs/macroeconomia/apostila.pdf) |
| 3 | Microeconomia | Carlos Eugênio Ellery Lustosa da Costa | [`docs/microeconomia/apostila.pdf`](docs/microeconomia/apostila.pdf) |
| 4 | Estatística | Eduardo Campos | [`docs/estatistica/apostila.pdf`](docs/estatistica/apostila.pdf) |
| 5 | Econometria | Marcelo Mello | [`docs/econometria/apostila.pdf`](docs/econometria/apostila.pdf) |

Cada apostila segue o mesmo padrão: a teoria como **método aplicado** — motivação econômica,
derivações passo a passo, diagramas em **TikZ** e **laboratórios computacionais em R** —
mais as **monitorias e listas resolvidas** de cada disciplina.

## Estrutura

```
.
├── README.md
└── docs/                       # site publicado via GitHub Pages
    ├── .nojekyll
    ├── index.html              # página-hub das disciplinas
    ├── assets/
    │   ├── styles.css          # folha de estilo compartilhada
    │   └── epge.png            # logo EPGE/FGV
    ├── matematica/
    │   ├── index.html
    │   └── apostila.pdf
    ├── macroeconomia/
    │   ├── index.html
    │   └── apostila.pdf
    ├── microeconomia/
    │   ├── index.html
    │   └── apostila.pdf
    ├── estatistica/
    │   ├── index.html
    │   └── apostila.pdf
    └── econometria/
        ├── index.html
        └── apostila.pdf
```

As apostilas são compiladas em Quarto (LaTeX + knitr) a partir dos repositórios de cada
disciplina; aqui ficam apenas os PDFs finais e o site que os apresenta. Novas disciplinas
do doutorado são acrescentadas seguindo a mesma estrutura.

## Publicar (GitHub Pages)

1. Crie um repositório e faça o push deste diretório.
2. Em **Settings → Pages**, selecione a branch `main` e a pasta `/docs`.
3. O site fica disponível em `https://<usuario>.github.io/<repo>/`.

Para atualizar uma apostila, recompile o PDF no repositório de origem e copie o novo
`index.pdf` para o `docs/<disciplina>/apostila.pdf` correspondente.

## Créditos

Notas de estudo de autoria de **Vítor Wilher**. Material de terceiros (livros-texto,
slides e listas originais das disciplinas) **não** é redistribuído aqui — apenas as notas
de autoria própria e as apostilas compiladas.
