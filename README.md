# Suicide FUT — Cartinhas da Temporada

Site estático de arquivo único (`index.html`): ranking com destaque dourado, cartinhas estilo FUT com foto, radar de atributos (SVG puro, sem bibliotecas) e poderes especiais + comentários da galera. Sem votos individuais — só médias.

## Estrutura de pastas

```
fut_suicide/
├── index.html
└── fotos/
    ├── martins.jpg
    ├── kelvin.jpg
    └── ...
```

## Fotos dos jogadores

Crie uma pasta `fotos/` ao lado do `index.html` e salve uma foto por jogador (de preferência quadrada — ela vira um círculo no card). O site procura primeiro `.jpg` e depois `.png`; se não achar, mostra as iniciais. Nomes exatos dos arquivos:

| Jogador | Arquivo |
|---|---|
| Andre | `andre.jpg` |
| Cesar | `cesar.jpg` |
| Claudio | `claudio.jpg` |
| Doardo | `doardo.jpg` |
| Felipe | `felipe.jpg` |
| Galvani | `galvani.jpg` |
| Guifosca | `guifosca.jpg` |
| Henrique | `henrique.jpg` |
| Kelvin | `kelvin.jpg` |
| Luan | `luan.jpg` |
| Lucca | `lucca.jpg` |
| Martins | `martins.jpg` |
| Moises | `moises.jpg` |
| Mozz | `mozz.jpg` |
| Pedro | `pedro.jpg` |
| Rix | `rix.jpg` |
| Willy | `willy.jpg` |

Tudo minúsculo, sem acento, com hífen no lugar de espaço.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (ex.: `suicide-fut`).
2. Suba o `index.html` **e a pasta `fotos/`** para a raiz (em **Add file → Upload files** dá pra arrastar a pasta inteira).
3. Vá em **Settings → Pages**.
4. Em **Source**, escolha **Deploy from a branch**; em **Branch**, `main` e `/ (root)`. Salve.
5. Em 1–2 minutos o site estará em `https://SEU_USUARIO.github.io/suicide-fut/`.

## Como atualizar as notas

Os dados ficam na constante `const DATA = {...}` dentro do `<script>` no `index.html`. Para uma nova rodada de votação é só regenerar esse bloco (ou me pedir de novo com a planilha nova).
