# polypodium-site

Site público do [Polypodium](https://github.com/bruno1pb13/Polypodium), servido via GitHub Pages.

- `privacidade.html` — Política de Privacidade (PT-BR), exigida pelo Google Play e pela Microsoft Store.
- `privacy.html` — Privacy Policy (EN).
- `index.html` / `index.en.html` — landing page (PT/EN) com recursos, capturas, download (Google Play, Microsoft Store, GitHub Releases para Linux) e perguntas frequentes.
- `self-host.html` / `self-host.en.html` — documentação técnica do servidor: instalação, HTTPS, build, workspaces e jardins, administração, previsão do tempo, rega pelo clima, MCP e referência da API. Mantenha as duas versões com as mesmas seções; o app abre essas URLs em "Ver documentação".
- `sitemap.xml` — inclui as alternativas de idioma (`hreflang`); atualize o `lastmod` ao mudar uma página.
- `assets/` — versões otimizadas dos arquivos do app: logo (`logo.png` é o original), fundo botânico (`background.webp`), ícones (`favicon-48`/`icon-192`/`apple-touch-icon`), `og-*.jpg` para compartilhamento e as fontes Cormorant Garamond em WOFF2 com só os caracteres latinos (`pyftsubset` a partir dos TTF do app).
- Capturas por idioma (`*-pt-*` / `*-en-*`), em WebP e em vários tamanhos para o `srcset`: `hero-*` (celular, claro e escuro, 1x/2x), `gallery-*` (quatro telas do celular) e `desktop-*`. Vêm das imagens das lojas em `Polypodium/docs/store/`, feitas com dados fictícios.

## SEO

- Edite os HTML localmente, não pelo editor web do GitHub: ele já truncou linhas longas com `[...]` e quebrou meta tags e ícones.
- Cada página tem `title`, `description`, `canonical`, `hreflang` e dados estruturados JSON-LD (`MobileApplication` e `FAQPage` na home). Ao mudar recursos do app, atualize também o `featureList` e o `softwareVersion`.
- Valide em https://search.google.com/test/rich-results e reenvie o sitemap no Search Console.

Quando o domínio próprio estiver ativo, basta configurá-lo como *custom domain* nas configurações do Pages — as URLs antigas do `github.io` redirecionam automaticamente.
