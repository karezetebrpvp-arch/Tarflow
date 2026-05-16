# Pasta `brand/` — Identidade Visual do Tarflow

Esta pasta concentra **todos** os arquivos visuais oficiais da marca Tarflow.
Sempre que precisar usar a logo (site, app, redes sociais, materiais impressos), pegue daqui.

---

## Estrutura

```
brand/
├── icon/                  ← Apenas o ícone (símbolo "T" com seta)
│   ├── tarflow_icon.svg          ← Vetorial — escala em qualquer tamanho
│   ├── tarflow_icon_512.png      ← (adicionar quando tiver o PNG real 512x512)
│   ├── tarflow_icon_192.png      ← (adicionar PNG 192x192)
│   ├── tarflow_icon_64.png       ← (adicionar PNG 64x64, para favicon)
│   └── tarflow_icon_apple.png    ← (180x180, para iOS)
│
├── logo/                  ← Logo completa (ícone + "Tarflow" + tagline)
│   ├── tarflow_logo.svg          ← Vetorial — versão completa
│   ├── tarflow_logo_full.png     ← (adicionar PNG quadrado alta resolução)
│   ├── tarflow_logo_horizontal.png  ← (adicionar versão horizontal, se houver)
│   ├── tarflow_logo_white.png    ← (adicionar versão sobre fundo claro)
│   └── tarflow_logo_dark.png     ← (adicionar versão sobre fundo escuro)
│
└── README.md              ← Este arquivo
```

---

## Como adicionar os PNGs reais

1. Copie os arquivos PNG que você gerou (os que aparecem nas duas imagens enviadas) para:
   - **Ícone sozinho** → `brand/icon/`
   - **Logo completa com texto** → `brand/logo/`

2. Renomeie seguindo o padrão acima (`tarflow_icon_512.png`, etc).

3. Avise para integrar no app — vou substituir o "T" estilizado pelo seu PNG real.

---

## Especificações de cor

| Elemento | Cor | Hex |
|---|---|---|
| Fundo do ícone (gradiente topo) | Azul royal | `#1e5fd4` |
| Fundo do ícone (gradiente base) | Azul profundo | `#0a3a96` |
| Letra T | Branco | `#ffffff` (com sombra suave) |
| Seta ascendente | Azul ciano gradiente | `#3aa3ff` → `#5ec8ff` |
| Texto "Tarflow" | Branco | `#ffffff` |
| Palavra "clareza" (tagline) | Azul claro | `#5ec8ff` |
| Fundo geral (manifesto) | Azul-marinho | `#0a1e3a` |

---

## Onde a logo é usada no app

- **Header da sidebar** → ícone pequeno (40x40)
- **Aba Sobre — Hero** → ícone grande (80x80)
- **Favicon do navegador** → 32x32
- **manifest.json** (PWA install) → 192x192 e 512x512
- **Apple touch icon** (iPhone) → 180x180
- **Notificações push** → 96x96
- **Splash screen** (futuro) → 1024x1024

---

## Tagline oficial

> **Controle suas finanças com clareza.**

---

## Versões SVG (provisórias)

Coloquei dois SVGs vetoriais reproduzindo aproximadamente o estilo das imagens que você criou:

- `icon/tarflow_icon.svg` — só o ícone
- `logo/tarflow_logo.svg` — ícone + texto + tagline

Esses SVGs servem como placeholder. Quando você adicionar os PNGs originais (que ficaram melhores que SVG manual), os PNGs viram a versão "principal" e o SVG fica como backup/uso vetorial.
