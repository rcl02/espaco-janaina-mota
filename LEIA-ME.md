# Site Espaço Janaina Mota

Landing page estática (HTML + CSS puro) que leva a cliente a agendar pelo WhatsApp.

## Arquivos

| Arquivo | O que é |
|---|---|
| `index.html` | Página inteira (estrutura, CSS e o pequeno script de animação) |
| `assets/img` | Fotos em WebP (480px e 850px), imagem de compartilhamento (OG) e ícones |
| `assets/fonts` | Cormorant Garamond, Jost e Pinyon Script (WOFF2, auto-hospedadas) |
| `_headers` | Regras de cache para o Cloudflare Pages |
| `robots.txt`, `sitemap.xml`, `favicon.ico`, `apple-touch-icon.png`, `site.webmanifest` | SEO e ícones |

## Antes de publicar

- Troque `https://espaco-janaina-mota.pages.dev/` pelo endereço final em `index.html`, `robots.txt` e `sitemap.xml` (procure por `✏️ CONFIRMAR`).
- **Trocar uma foto**: gere `nome-480.webp` e `nome-850.webp` em `assets/img` e atualize `src`/`srcset` da `<img>`. Mantenha `width`/`height` com o tamanho real.
- Os dados do negócio para o Google (endereço, horários, telefone) ficam no bloco `application/ld+json` do `<head>`; se mudar no site, mude lá também.

## Publicar grátis no Cloudflare Pages

Cloudflare → Workers & Pages → Create → Pages → **Upload assets** → arraste esta pasta → Deploy.
