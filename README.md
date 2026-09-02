# Zsóri Ádám – személyes weboldal

Egyetlen statikus `index.html` fájl, build lépés nélkül – bárhová deployolható.

## Deploy Cloudflare Pages-re

### A) Legegyszerűbb: drag & drop
1. Menj a [Cloudflare Dashboard](https://dash.cloudflare.com/) → **Workers & Pages** → **Create** → **Pages** → **Upload assets**.
2. Adj nevet a projektnek (pl. `zsori-adam`), majd húzd be ezt a mappát (vagy az `index.html`-t).
3. Kész – kapsz egy `*.pages.dev` címet. Saját domaint a projekt **Custom domains** fülén tudsz kötni hozzá.

### B) Git-alapú (automatikus deploy minden pushnál)
1. Tedd fel a mappát egy GitHub repóba.
2. Cloudflare Dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
3. Válaszd ki a repót, build parancs: *nincs*, output könyvtár: `/`.

### C) Parancssorból (wrangler)
```bash
npm install -g wrangler
wrangler login
wrangler pages deploy . --project-name zsori-adam
```

## Amit később kell pótolni (a fájlban `TODO` kommentekkel jelölve)

- **Profilkép:** tegyél a mappába egy `profile.jpg`-t, és a hero szekcióban cseréld a monogramos div-et a kommentben megadott `<img>` tagre.
- **Everest Accounting:** mit csinálsz pontosan + használt technológiák (tapasztalat szekció).
- **Projektek:** további projekt kártyák (a "Hamarosan…" kártyák helyére).
- **Vállalkozás:** név, bemutatkozó szöveg, tényleges szolgáltatások.
- **GitHub / LinkedIn linkek:** a kapcsolat szekció alján lévő ikonok `href`-jei.
- **Oracle dátum:** jelenleg "2023 – 2025" szerepel – igazítsd, ha nem pontos.
