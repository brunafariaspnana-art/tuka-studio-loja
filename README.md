# Tukã Studio · Loja virtual

Loja da Tukã Studio (Coleção Caveiras). Site estático: HTML, CSS e JavaScript puro, sem build e sem dependências.

## Estrutura

```
index.html        página da loja (estilos e scripts inclusos)
assets/logo.webp  logo
assets/placa.webp foto da placa iluminada
vercel.json       configuração da Vercel
```

## Rodar localmente

Abra o `index.html` no navegador, ou rode `npx serve .` na pasta.

## Publicar no GitHub

```bash
git init
git add .
git commit -m "Loja Tukã Studio"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/tuka-studio-loja.git
git push -u origin main
```

## Publicar na Vercel

1. Entre em vercel.com, clique em **Add New → Project** e importe o repositório.
2. Framework Preset: **Other**. Deixe Build Command e Output Directory em branco.
3. Clique em **Deploy**.

## O que editar no `index.html`

- **Produtos e preços:** procure por `const P=[`. Cada item tem nome, preço (`price`), preço antigo (`old`), modelagem e estoque por tamanho.
- **Cupons:** procure por `const COUPONS=`.
- **Frete grátis:** `const FREE=299;`
- **WhatsApp:** troque `5500000000000` pelo número com DDI e DDD (ex.: `5511999998888`).
- **Instagram:** troque `tukastudio` em `instagram.com/tukastudio`.
- **CNPJ, e-mail e telefone:** no rodapé (`<footer>`).

## Pagamentos

O checkout é de demonstração: não cobra nada e não envia dados. Para vender de verdade, integre um gateway (Mercado Pago, Pagar.me, PagSeguro, Stripe) ou use uma plataforma como Nuvemshop ou Shopify.
