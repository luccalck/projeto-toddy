# Projeto Toddy

Site institucional fictício da marca Toddy, desenvolvido como projeto de ADS — SENAI.

## Stack

- HTML estático
- Tailwind CSS (via CDN)
- JavaScript vanilla
- Vídeos `.mp4` controlados por scroll e em loop autoplay

## Estrutura

```
ProjetoToddy/
├── index.html      # Página única (SPA estática)
└── video/          # Vídeos e imagens de produto
    ├── TODDYUSAR_scrub.mp4    # Hero — scroll-controlled
    ├── ToddyFullFrames.mp4    # Toddy Original — autoplay loop
    └── toddyblack169.png      # Toddy Dark
```

## Funcionalidades

- Hero com vídeo controlado por scroll (scrub)
- Animações de fade-in/out bidirecionais ao rolar
- 3 produtos + 3 combos com preços
- Carrinho em drawer com quantidade, total e persistência via `localStorage`
- Login simples (nome + e-mail) com validação
- Confirmação de pedido com número de referência gerado
- Logout no navbar quando logado
- Newsletter com validação de e-mail
- Scrollbar visualmente oculta, scroll suave em toda a página

## Como rodar localmente

Por causa dos vídeos, é preciso servir via HTTP (não abrir o arquivo direto):

```bash
python -m http.server 5181
# abrir http://localhost:5181
```

## Deploy

Site estático — funciona direto no Vercel, Netlify ou GitHub Pages sem build step.
