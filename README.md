# Administração com IA na Prática

Página estática, sem dependências e sem etapa de compilação.

## Arquivos e caminhos

- `index.html`: página inicial; edite este arquivo para atualizar o site.
- `administracao-com-ia-pagina-de-vendas.html`: arquivo original enviado, preservado.
- Imagens e estilos estão incorporados no HTML. Apenas as fontes usam Google Fonts.

## Netlify

No site existente, conecte este repositório, selecione a branch `main`, deixe o diretório base e o comando de build vazios e use `.` como diretório de publicação. O `netlify.toml` define a publicação a partir da raiz. Se o site foi enviado manualmente, faça um novo deploy da pasta que contém `index.html`.

Os caminhos `/`, `/index.html`, `/administracao-com-ia` e o endereço HTML antigo abrem a página. Os dois últimos redirecionam para `/` no Netlify. Não há regras genéricas que escondam erros 404.

## GitHub Pages

Em Settings → Pages → Build and deployment, selecione **GitHub Actions**. O workflow `.github/workflows/pages.yml` publica a cada push na branch `main`; depois da ativação, também pode ser iniciado em Actions → Publicar GitHub Pages → Run workflow.

Endereço esperado após a publicação: https://andersonx553-beep.github.io/EbookADM/

## Verificação local

Execute `python3 -m http.server 8080 --directory /workspace/EbookADM` e confira a página inicial, as imagens, as perguntas frequentes e o botão de copiar prompt. Em tarefas na nuvem, use o checkout existente; não é necessário criar worktrees.

## Pagamento

O HTML original não contém um link de pagamento. Configure `CHECKOUT_URL` no `index.html` com a URL real do checkout antes de começar a vender. Até isso acontecer, os botões levam à seção de oferta e não processam pagamentos.
