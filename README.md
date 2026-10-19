# Special Core — Sharkot

Site estático para GitHub Pages com as páginas:
- `index.html`: apresentação do Sharkot e catálogo pesquisável de comandos.
- `perfil.html`: prévia visual de perfil.
- `premium.html`: benefícios e solicitação manual de Premium.
- `admin.html`: protótipo local de gestão de VIP e permissões.
- `style.css`: identidade visual compartilhada.
- `special core image.png` e `special core admin.jpg`: imagens do projeto (adicione/substitua conforme as referências finais).

## Publicar no GitHub Pages
1. Envie os arquivos para a raiz do repositório.
2. No GitHub, abra **Settings → Pages**.
3. Em Build and deployment, selecione **Deploy from a branch**, escolha a branch principal e a pasta `/ (root)`.
4. Salve e aguarde a publicação.

## Antes de publicar
- Em `premium.html`, substitua `COLOQUE_SEU_CONVITE_DO_SERVIDOR_AQUI` pelo convite permanente do seu servidor Discord.
- O link OAuth2 para adicionar o bot já está configurado em `index.html`. Ele é diferente do convite do servidor.
- Confira se o nome dos arquivos e maiúsculas/minúsculas coincidem exatamente com os nomes no GitHub.

## Limites importantes desta versão
Este projeto é front-end estático. A página de perfil só faz uma prévia no navegador e salva cores no `localStorage`. O painel admin guarda registros localmente no navegador de quem o abre; não verifica o Gmail, não protege acessos reais e não altera dados do bot. Não use os registros locais como prova de compra ou como controle de acesso em produção.

Para produção, implemente autenticação Google (OAuth/OpenID Connect) e um backend/API que valide a identidade e as permissões no servidor. O backend deve proteger ações administrativas e integrar-se ao banco de dados do Sharkot. Nunca coloque token do Discord, segredo OAuth ou credenciais no HTML/JavaScript público.

## Créditos
Feito por 7mr.sam7. © Todos os direitos reservados. Special Core™.
