# mayge.us

Convite de casamento de **Mayara e Gêdhean** — 28 de novembro de 2026, Montepascual Ecovillage, Lagoinha, Ceará.

Site publicado em <https://mayge.us>.

## Stack

HTML e CSS puro. Sem build, sem dependências, sem JavaScript.

Todas as ilustrações (coqueiros, praia, corações) e ícones são SVG inline
desenhados à mão via `<symbol>` / `<use>` — não há imagens externas.

| Arquivo | Conteúdo |
| --- | --- |
| `index.html` | Estrutura semântica e definições SVG |
| `styles.css` | Design tokens, layout (Grid/Flexbox), responsivo e print |
| `CNAME` | Domínio customizado do GitHub Pages |
| `.nojekyll` | Desativa o Jekyll (serve os arquivos como estão) |

## Desenvolvimento local

Basta abrir o arquivo:

```sh
open index.html
```

Ou servir via HTTP (útil para testar no celular na mesma rede):

```sh
python3 -m http.server 8731
```

## Tipografia

Carregada do Google Fonts, com fallbacks locais:

- **Cormorant Garamond** — títulos e nomes
- **Jost** — texto corrido
- **Parisienne** — assinatura "Contamos com vocês!"

## Deploy

GitHub Pages serve a branch `main` (raiz). Todo push para `main` publica
automaticamente — não há workflow de build.

## Responsivo

- `> 860px` — três colunas, divisores verticais
- `≤ 860px` — colunas empilhadas, divisores horizontais
- `≤ 520px` — botões em largura total, textos refluídos
