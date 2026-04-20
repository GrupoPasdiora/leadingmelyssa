# Diagnóstico ELO — Mel Figueiredo

Landing page estática da mentora Mel Figueiredo para o produto Diagnóstico ELO.

## Arquivos

- `index.html` — página completa, todas as fotos e prints embutidos em base64
- `depoimento-video.mp4` — vídeo de depoimento exibido na seção "Quem viveu, sentiu"
- `mensagem-mel.mp4` — vídeo da Mel exibido na seção de Autoridade
- `README.md` — este arquivo

**Importante:** os três arquivos MP4 e o HTML precisam estar na mesma pasta.
O HTML referencia os vídeos via caminho relativo (`./depoimento-video.mp4` e
`./mensagem-mel.mp4`).

## Como publicar no GitHub Pages

1. Crie um repositório público (ex.: `melfigueredo-site`).
2. Faça upload de TODOS os arquivos deste pacote na raiz do repositório.
3. Vá em **Settings → Pages**.
4. Em **Source**, selecione **Deploy from a branch**.
5. Escolha a branch `main` e a pasta `/ (root)`. Salve.
6. Aguarde 1–2 minutos. A URL aparece no topo da mesma página
   (ex.: `https://seuusuario.github.io/melfigueredo-site/`).
7. Para usar domínio próprio (ex.: `melfigueredo.shop`):
   - Em **Pages → Custom domain**, digite o domínio e salve.
   - No painel do seu provedor de domínio, crie um registro CNAME
     apontando para `seuusuario.github.io`.

## Atualizar conteúdo

O `index.html` é autônomo — as imagens estão dentro dele em base64.
Para trocar uma foto, gere o novo base64 (`base64 -w0 foto.jpg`) e
substitua o trecho `data:image/jpeg;base64,...` correspondente.

Para trocar um vídeo, substitua o arquivo `.mp4` mantendo o mesmo nome.

## CTA / Pagamento

O botão "Fazer meu Diagnóstico ELO" aponta para:
`https://pay.cakto.com.br/38ru8or_852246`

Se mudar o link da Cakto, faça find/replace por essa URL no HTML.

## Atenção ao cache

Depois de fazer upload de uma nova versão, o navegador pode continuar
mostrando a versão antiga por causa do cache. Faça um hard refresh:
- Mac: `Cmd + Shift + R`
- Windows: `Ctrl + Shift + R` (ou `Ctrl + F5`)

Se tiver domínio próprio atrás de CDN (Cloudflare, etc.), a atualização
pode levar alguns minutos adicionais.

---

© 2026 Mel Figueiredo · Mentora de Mulheres
