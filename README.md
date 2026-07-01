# Alfahone - Site Institucional

Site institucional estático da Alfahone, focado em conversão para contato comercial via WhatsApp, com SEO técnico, acessibilidade e performance.

## Tecnologias usadas
- HTML5 semântico
- CSS3 moderno (sem framework pesado)
- JavaScript moderno (vanilla JS)
- Google Fonts (Inter)

## Estrutura de pastas
```text
/
|-- index.html
|-- robots.txt
|-- sitemap.xml
|-- manifest.webmanifest
|-- README.md
`-- assets/
    |-- scripts/
    |   `-- main.js
    |-- styles/
    |   `-- main.css
    `-- images/
        |-- brand/
        |   |-- logo-full.png
        |   `-- logo-symbol.png
        |-- icons/
        |   |-- app-icon-192.svg
        |   |-- app-icon-512.svg
        |   |-- favicon.svg
        |   |-- flow-chat.png
        |   `-- whatsapp-floating.svg
        `-- social/
            `-- open-graph.svg
```

## Como rodar localmente
1. Abra a pasta do projeto.
2. Execute um servidor estático local (ex.: extensão Live Server no VS Code).
3. Acesse a URL local exibida pelo servidor.

## Como publicar em hospedagem estática
1. Envie todos os arquivos para a raiz do domínio `https://alfahone.com.br`.
2. Garanta que `index.html`, `robots.txt`, `sitemap.xml` e `manifest.webmanifest` estejam na raiz.
3. Valide o HTTPS e o carregamento dos recursos em `/assets`.

## Checklist de SEO
- [x] `title` otimizado
- [x] `meta description`
- [x] `meta keywords` moderada
- [x] canonical em `https://alfahone.com.br/`
- [x] `robots` index/follow
- [x] Open Graph
- [x] Twitter Cards
- [x] JSON-LD (`Organization`)
- [x] `sitemap.xml`
- [x] `robots.txt`
- [x] Hierarquia correta de headings e apenas um H1

## Checklist de segurança
- [x] Sem `eval`
- [x] Sem dependências externas desnecessárias
- [x] Links externos com `rel="noopener noreferrer"`
- [x] Sem chaves/tokens no front-end
- [x] Sem formulário com coleta sensível
- [x] Contato principal via WhatsApp
- [x] Meta CSP básica implementada no HTML

### Headers HTTP recomendados para produção
- `Content-Security-Policy`
- `X-Content-Type-Options: nosniff`
- `Referrer-Policy: strict-origin-when-cross-origin`
- `Permissions-Policy`
- `Strict-Transport-Security` (apenas em HTTPS)

## Checklist de performance
- [x] CSS e JS enxutos
- [x] Scripts com `defer`
- [x] Sem bibliotecas pesadas
- [x] Layout responsivo mobile-first
- [x] Animações leves via CSS/IntersectionObserver
- [x] Assets visuais locais e enxutos

## Observações
- Este projeto não possui backend.
- Não há coleta de dados sensíveis.
- Recomenda-se rodar Lighthouse antes da publicação final para ajustes finos por ambiente.
