# Agência Criativa Web — Refatoração com SASS

Landing page de uma agência de design digital, refatorada para uma arquitetura modular e escalável utilizando SASS/SCSS.

## Objetivo

Transformar o CSS tradicional do projeto em um sistema organizado com partials, variáveis, mixins, aninhamento e operadores, mantendo total responsividade e seguindo a metodologia BEM.

## Estrutura SASS

O projeto foi dividido em arquivos parciais com responsabilidades bem definidas, todos importados e compilados pelo arquivo principal `estilos.scss`:

- `_variaveis.scss` — cores, tipografia e espaçamentos globais
- `_base.scss` — reset e estilos globais de html/body
- `_mixins.scss` — mixins reutilizáveis: `divisor`, `image`, `button`
- `_layout.scss` — posicionamento e estrutura de cada seção
- `_componentes.scss` — componentes isolados como botões
- `_animacoes.scss` — transições e efeitos de hover
- `_responsividade.scss` — media queries para todos os breakpoints

## Recursos SASS aplicados

**Variáveis** para cores (`$primary-color`), família e tamanhos de fonte (`$font-title`, `$font-big`, `$font-medium`, `$font-small`) e espaçamento base (`$espacamento`).

**Mixins** reutilizados em múltiplos componentes: `image` eliminou a duplicação entre `.imagem-desktop` e `.imagem-form`; `button` centraliza os estilos base de todos os botões; `divisor` gera os separadores de seção via `::before`.

**Operadores** para cálculos proporcionais, como `variaveis.$espacamento * 5` na seção de contato.

**Aninhamento** com `&` aplicado de forma moderada, respeitando a nomenclatura BEM para manter o CSS gerado limpo e sem especificidade excessiva.

## Tecnologias

HTML5, SASS/SCSS, CSS3 (Grid e Flexbox), JavaScript Vanilla, Swiper JS e Font Awesome.

## Como visualizar

Clone o repositório, certifique-se de que a pasta `img/` contém as imagens necessárias e abra o `index.html` em qualquer navegador moderno. O CSS já está compilado na pasta `CSS/`.
