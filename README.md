# Módulo 06 · Turma T17 · Inteli 2026.1B

Repositório com as apresentações do módulo Plataforma digital baseada em arquitetura
orientada a serviços da turma T13 do Inteli.

## Como abrir

Abra `aulas/index.html` em um navegador moderno, ou rode um servidor local:

```bash
npx serve aulas
```

Depois navegue até `http://localhost:3000`.

## Estrutura

```
aulas/
├── assets/
│   ├── css/
│   │   ├── inteli-theme.css        tema Reveal com paleta Inteli
│   │   └── inteli-print.css        estilos de impressão (PDF)
│   ├── img/
│   └── js/
│       ├── inteli-pdf-exports.js   pdf export
│       ├── inteli-quiz.js          quiz interativo
│       ├── inteli-timer.js         timer 
│       └── inteli-zoom.js          zoom em imagens
├── aula02.html                     Filtragem Colaborativa por Usuário (27/04)
├── aula03.html                     Projeto de Software orientado a objetos (28/04) 
├── index.html
└── index.md
```

## Cronograma

### Sprint 1 · Descoberta · 22/04 a 30/04

| Aula | Data | Tema |
|------|------|------|
| 01 | 23/04 (qui) | Filtragem Colaborativa baseada em Item |
| 02 | 27/04 (seg) | Filtragem Colaborativa por Usuário |
| 03 | 28/04 (ter) | Projeto de Software orientado a objetos: conceito de entidades, propriedades, separação de contextos e diagrama UML de classes |

### Sprint 2 · Projeto · 04/05 a 15/05

| Aula | Data | Tema |
|------|------|------|
| 04 | 06/05 (qua) | Sistemas de recomendação baseados em filtragem colaborativa |
| 05 | 13/05 (qua) | Arquitetura Geral e Orientada a Serviços (SOA) e a perspectiva de requisitos não funcionais |

### Sprint 3 · Projeto · 18/05 a 29/05

| Aula | Data | Tema |
|------|------|------|
| 06 | 20/05 (qua) | Tópicos de BD: Stored Procedures e Functions |
| 07 | 22/05 (sex) | Tópicos de BD: Transactions e Triggers |
| 08 | 25/05 (seg) | FrontEnd Mobile e Arquitetura MVVM (React Native) |
| 09 | 28/05 (qui) | Orientação a objetos com TDD |

### Sprint 4 · Projeto · 01/06 a 12/06

| Aula | Data | Tema |
|------|------|------|
| 10 | 08/06 (seg) | Testes de Integração |
| 11 | 09/06 (ter) | Boas práticas para arquiteturas orientadas a serviço na nuvem |

### Sprint 5 · Projeto · 15/06 a 26/06

| Aula | Data | Tema |
|------|------|------|
| 12 | 16/06 (ter) | Monitoramento e logging: Técnicas de monitoramento de desempenho e logging em tempo real para serviços em nuvem |
| 13 | 23/06 (ter) | Segurança em sistemas distribuídos: Princípios de segurança aplicados a serviços na nuvem e APIs |
| 14 | 25/06 (qui) | Tópicos extras em paradigmas de programação - Padrões AutoML em dotnet |

## Identidade visual

O tema usa a paleta institucional Inteli:

- Purple `#2e2640`
- Coral `#ff4545`
- Lilac `#90a5e5`
- Green `#89cea5`
- Dark green `#066d73`

Tipografia: Manrope para texto e Space Mono para código.

A wordmark `inteli.` é renderizada em CSS enquanto não há arquivos PNG/SVG
oficiais na pasta `aulas/assets/img/`.

## Scripts

```bash
npm install         # instala Husky e Prettier
npm run lint        # valida formatação de md/yml/yaml/json
npm run format      # aplica formatação automaticamente
```

O hook `pre-commit` roda `lint-staged` antes de cada commit.

## Publicação

O workflow `.github/workflows/deploy-pages.yml` publica o conteúdo da pasta
`aulas/` no GitHub Pages a cada push em `main`.

Para ativar a primeira vez: em Settings, Pages, escolha a source "GitHub Actions".

## Estado atual

Os esqueletos das aulas 02 e 03 estão criados, com capa, agenda, objetivos,
separadores de bloco, slide de exercício, quiz, auto-estudo e encerramento.
O conteúdo detalhado (slides internos de fundamentos e práticas) será populado
aula por aula.
