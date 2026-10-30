# SAVA — Landing do anúncio

Página única (`index.html` + `img/`), sem build. Publicada pelo GitHub Pages em
https://lp.savatecnologia.com.br (arquivo `CNAME`). Todo push na `main` publica.

- O formulário grava na tabela `inscricoes` do Supabase da SAVA Gestão
  (`lina-gestao/supabase/inscricoes.sql`). A chave `anon` no HTML é pública por desenho.
- Prévia privada: `<script>window.SAVA_PREVIA = true</script>` antes do script principal faz o
  formulário NÃO gravar. Nunca publicar com essa linha.
- Pixel da Meta: preencher `META_PIXEL_ID` no `index.html` (vazio = não carrega).
- Origem: artifact "Landing do anúncio SAVA" do claude.ai, trazido em 29/10/2026.

## Git: absolutamente tudo é salvo — commit E push — sem perguntar

- Toda mudança que deixa o projeto funcionando vira **commit e push** na mesma sessão, logo
  depois de feita. Não perguntar "quer que eu faça o commit?".
- **Nunca** vai pro git: segredo e credencial (`.env`, `*.local`, chaves, tokens), dado real
  de cliente.
- Ainda pedir confirmação antes de: force-push, reescrever histórico, apagar branch.
- Aqui push na `main` = publicar em produção; o Pedro autorizou publicar esta landing em
  30/10/2026, mas mudança grande de conteúdo/oferta: mostrar antes.
