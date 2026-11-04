# Administração com IA na Prática • Lia

Página de vendas atualizada enviada pelo usuário. Há uma única página pública, `index.html`, com estilos e imagens incorporados. Fontes são carregadas pelo Google Fonts.

## Navegação e pagamento

Chamadas do cabeçalho, conteúdo e barra móvel descem suavemente até `#oferta`. Somente o botão principal “Comprar agora” dessa seção abre https://pay.kiwify.com.br/Sb1GbMt. A preferência de movimento reduzido é respeitada. O botão de copiar prompt e as perguntas frequentes funcionam sem dependências.

## Netlify

Repositório: andersonx553-beep/EbookADM. Branch: main. Diretório base vazio; comando de build vazio; diretório de publicação: `.`. O arquivo `netlify.toml` configura a raiz e redireciona os dois nomes HTML anteriores e o caminho `/administracao-com-ia` para `/`. A página antiga foi removida do checkout.

Com deploy automático habilitado, o push na main dispara a publicação. Para deploy manual, envie a raiz contendo index.html e netlify.toml. Não envie apenas uma pasta vazia ou a pasta de produção do PDF. O produto pago não está neste repositório.

## GitHub Pages

O workflow publica somente index.html e .nojekyll. Configure Settings → Pages → GitHub Actions. Os redirects do netlify.toml são exclusivos do Netlify; no Pages, use a raiz do projeto.

## Desenvolvimento

Use o checkout existente; não é necessário criar worktrees. Execute `python3 -m http.server 8080 --directory /workspace/EbookADM` para verificar localmente.
