# TiPCA Lab - site público

Código dos componentes HTML do site público do TiPCA Lab.

**Linha de pesquisa única:** Sistemas Elétricos, Automação, Controle e Tecnologias Inteligentes.

## Estrutura

- `home/pic-destaque/`: destaque temporário do PIC 2027.
- `home/restante/`: restante da Home. **Pendente inserir o HTML consolidado `02_home_restante_v1.0`.**
- `pic/2027/`: página do processo seletivo PIC 2027.
- `pesquisa/projetos/`: página de Projetos de Pesquisa.
- `noticias/`, `eventos/`, `recursos/`: conteúdo futuro.
- `assets/`: logos, imagens e posteriormente CSS compartilhado.
- `archive/`: snapshots especiais; versões normais ficam no histórico Git.

## Fluxo

- `main`: conteúdo publicado.
- Commits: `feat:`, `fix:`, `content:`, `style:`, `chore:`.
- Não use nomes como `final2`; use o histórico Git.

## Publicação

Estrutura preparada para GitHub Pages. Cada componente usa `index.html`, produzindo URLs estáveis para incorporação no Google Sites.

## Segurança

Não inclua dados pessoais de estudantes, candidatos, documentos internos, tokens, chaves ou credenciais.
