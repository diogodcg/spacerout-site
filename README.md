# spacerout-site

Site institucional do SpaceRout (`spacerout.com.br`): apresentação, perguntas
frequentes, política de privacidade e termos, e a página de exclusão de conta
e dados. É só HTML/CSS estático, sem scripts.

Este repositório é público **de propósito** e só contém o conteúdo do site. O
código do aplicativo fica em outro repositório, privado.

## Estrutura

- `public/` — as páginas e os arquivos de estilo/ícones que vão ao ar
- `public/_headers` — cabeçalhos de segurança (HSTS, CSP restrita etc.)
- `wrangler.jsonc` — configuração do deploy na Cloudflare (pasta `public/`)

## Publicação

A Cloudflare publica a pasta `public/` automaticamente a cada push na `main`.
As URLs abaixo são usadas pelo aplicativo e pela ficha da Google Play, então
**não devem mudar de caminho**:

- `/privacidade.html`
- `/exclusao-de-conta.html`
- `/faq.html`

Não versione segredos, chaves ou dados de usuários aqui.
