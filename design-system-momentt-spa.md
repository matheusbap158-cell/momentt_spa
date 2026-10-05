# Design System - Momentt Spa

Base extraída da logo real (flor de lótus dourada com relevo, sobre fundo escuro) e do perfil @momentt_spa. Tom: luxo acolhedor, calmo, feminino sem ser infantil.

## Resumo do tom visual
- Preto quente (marrom quase preto) com dourado champagne: sofisticado e quente, nunca frio.
- Muito respiro, títulos em serifa elegante e itálico dourado para a palavra de destaque.
- Linhas finas douradas e a flor de lótus como ornamento; sem sombras pesadas.

## 1. Cores

| Token | Hex | Uso |
|---|---|---|
| --noir-950 | #0F0C09 | Fundo do hero, rodapé e blocos escuros |
| --noir-900 | #17120D | Fundo de seção escura alternada |
| --noir-800 | #221A12 | Cards sobre fundo escuro |
| --gold-300 | #E6CC8A | Destaque de palavra (itálico) em fundo escuro |
| --gold-400 | #D4AF5F | Linhas, ícones, bordas ativas |
| --gold-500 | #C09A45 | Cor de ação: botão primário |
| --gold-700 | #7D5F22 | Texto dourado sobre fundo claro (contraste AA em marfim) |
| --ivory-50 | #FAF5EA | Fundo claro padrão |
| --ivory-100 | #F1E8D6 | Seção clara alternada |
| --ivory-200 | #E2D5BC | Bordas e divisores em fundo claro |
| --ink-900 | #1D1710 | Texto principal em fundo claro |
| --ink-600 | #5F5444 | Texto secundário em fundo claro |
| --text-on-dark | #EADFC9 | Texto principal em fundo escuro |
| --text-on-dark-muted | #BFB197 | Texto secundário em fundo escuro |
| --wa-500 | #25D366 | EXCLUSIVO do botão de WhatsApp |

Contrastes: #EADFC9 sobre #0F0C09 acima de 13:1; #1D1710 sobre #FAF5EA acima de 15:1; #5F5444 sobre #FAF5EA acima de 6:1; #17120D sobre #C09A45 acima de 6:1.

## 2. Tipografia (Google Fonts)
- Títulos: Cormorant Garamond (500 e 600, itálico para destaque). Parece com a serifa da logo.
- Corpo e botões: Jost (400, 500, 600).

| Nível | Desktop | Mobile | Peso | Entrelinha | Espaçamento |
|---|---|---|---|---|---|
| H1 | 68px | 42px | 500 | 1.05 | -0.01em |
| H2 | 46px | 32px | 500 | 1.12 | -0.005em |
| H3 | 26px | 23px | 600 | 1.2 | 0 |
| Eyebrow | 12.5px | 12px | 500 | 1.4 | 0.22em, maiúsculas |
| Corpo | 17px | 16px | 400 | 1.75 | 0 |
| Botão | 15px | 15px | 600 | 1 | 0.04em |

## 3. Componentes
- **Botão primário:** gradiente dourado (#D4AF5F para #C09A45), texto #17120D, raio 999px (pílula), altura mínima 52px. Hover: sobe 2px e clareia. Foco: contorno dourado de 3px com 3px de afastamento.
- **Botão secundário:** transparente, borda dourada de 1px, texto marfim. Hover: fundo dourado a 10%.
- **Botão WhatsApp (verde):** só no botão flutuante e na seção de contato.
- **Card escuro:** fundo #221A12, borda 1px dourada a 22%, raio 20px. Hover: borda dourada a 60%.
- **Input:** fundo transparente, borda 1px #E2D5BC (claro) ou dourada a 30% (escuro), raio 14px, altura 52px. Foco: borda #C09A45 e contorno visível. Erro: borda #B3492E com texto de ajuda.

## 4. Estética
- Raios: 14px (campos), 20px (cards), 999px (botões e selos).
- Sombras: quase nenhuma; apenas brilho dourado suave em botão (0 8px 30px rgba(192,154,69,.25)).
- Espaçamento: escala de 8px (8, 16, 24, 32, 48, 72, 112). Seções com 112px de respiro no desktop e 72px no mobile.
- Ornamento: linha fina dourada com a flor de lótus ao centro entre seções.

## 5. Conversão para WhatsApp
- CTA dourado com ícone de WhatsApp no hero, após tratamentos e na chamada final. Verde só no flutuante e no contato.
- Verbos específicos: "Agendar minha avaliação pelo WhatsApp".
- Autoridade: nota 5,0 e 35 avaliações logo acima da dobra, avaliações reais com nome.
- Sem promessa de resultado; reforçar "avaliação individual".

## Tokens prontos (CSS)
```css
:root{
  --noir-950:#0F0C09; --noir-900:#17120D; --noir-800:#221A12;
  --gold-300:#E6CC8A; --gold-400:#D4AF5F; --gold-500:#C09A45; --gold-700:#7D5F22;
  --ivory-50:#FAF5EA; --ivory-100:#F1E8D6; --ivory-200:#E2D5BC;
  --ink-900:#1D1710; --ink-600:#5F5444;
  --text-on-dark:#EADFC9; --text-on-dark-muted:#BFB197;
  --wa-500:#25D366; --alert-600:#B3492E;
  --font-display:'Cormorant Garamond',Georgia,serif;
  --font-body:'Jost',-apple-system,'Segoe UI',sans-serif;
  --r-field:14px; --r-card:20px; --r-pill:999px;
}
```
