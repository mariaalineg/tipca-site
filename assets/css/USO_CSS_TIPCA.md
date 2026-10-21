# Uso do CSS compartilhado do TiPCA

Coloque o arquivo em:

```text
tipca-site/assets/css/tipca.css
```

Em páginas como `equipe/index.html` ou `pesquisa/index.html`, use:

```html
<link rel="stylesheet" href="../assets/css/tipca.css">
```

Em páginas dois níveis abaixo, como `pesquisa/projetos/index.html`, use:

```html
<link rel="stylesheet" href="../../assets/css/tipca.css">
```

Em páginas três níveis abaixo, como `pesquisa/projetos/cubesat/index.html`, use:

```html
<link rel="stylesheet" href="../../../assets/css/tipca.css">
```

Para evitar problemas de caminhos dentro do Google Sites, também é possível usar a URL absoluta:

```html
<link rel="stylesheet" href="https://mariaalineg.github.io/tipca-site/assets/css/tipca.css">
```

## Exemplo mínimo

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Página | TiPCA Lab</title>
  <link rel="stylesheet" href="https://mariaalineg.github.io/tipca-site/assets/css/tipca.css">
</head>
<body>
  <main class="tipca-container">
    <header class="tipca-page-header">
      <div class="tipca-kicker">TiPCA Lab</div>
      <h1>Título da página</h1>
      <p>Descrição breve e objetiva.</p>
    </header>

    <section class="tipca-section tipca-grid-2">
      <article class="tipca-card">
        <h2>Primeiro bloco</h2>
        <p>Conteúdo.</p>
        <a class="tipca-link" href="#">Mais informações →</a>
      </article>
      <article class="tipca-card">
        <h2>Segundo bloco</h2>
        <p>Conteúdo.</p>
      </article>
    </section>
  </main>
</body>
</html>
```

## Classes principais

- `.tipca-container`: largura e margens da página.
- `.tipca-section`: espaçamento entre seções.
- `.tipca-page-header`: cabeçalho interno da página.
- `.tipca-kicker`: rótulo superior de seção.
- `.tipca-grid-2` e `.tipca-grid-3`: grades responsivas.
- `.tipca-card` e `.tipca-card-compact`: cards.
- `.tipca-button`, `.tipca-button-primary`, `.tipca-button-secondary`, `.tipca-button-danger`: botões.
- `.tipca-link`: link editorial.
- `.tipca-badge`, `.tipca-badge-alert`, `.tipca-badge-success`: etiquetas.
- `.tipca-banner`: destaque com fundo roxo.
- `.tipca-callout`: aviso em fundo claro.
- `.tipca-research-line`: destaque da linha de pesquisa.
- `.tipca-person-card` e `.tipca-avatar`: equipe e participantes.
- `.tipca-project-card`: projetos comparáveis.
- `.tipca-footer`: rodapé interno.

## Migração recomendada

Faça a migração página por página. Em cada HTML:

1. adicione o `<link>` do CSS;
2. aplique as classes `tipca-*`;
3. remova do `<style>` local apenas as regras já cobertas pelo arquivo compartilhado;
4. mantenha localmente apenas regras realmente exclusivas da página;
5. teste no GitHub Pages e no Google Sites, especialmente no celular.
