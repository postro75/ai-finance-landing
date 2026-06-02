# AI & Finance — Landing Page

Statyczna strona HTML, zdeployowana na Vercel.

## Struktura
```
.
├── index.html          # Główna strona
├── images/             # Zdjęcia eksperta
│   ├── expert-houndstooth.jpg   # Hero
│   ├── expert-shirt.jpg         # Sekcja "O ekspercie"
│   ├── expert-fullbody-gray.jpg # Blog / press
│   └── expert-portrait-id.jpg   # Avatar / favicon
├── vercel.json         # Konfiguracja Vercel (cache, headers)
└── package.json        # npm scripts
```

## Lokalne uruchomienie
```bash
npm run dev
# lub
npx serve . -l 3000
```

## Deploy na Vercel

### Pierwszy deploy
```bash
vercel              # preview
vercel --prod       # produkcja
```

### Szybki deploy przez GitHub
1. Wgraj repo na GitHub
2. Import w Vercel dashboard → vercel.com/new
3. Framework Preset: **Other**
4. Build Command: *(puste)*
5. Output Directory: `.`
6. Deploy

## Custom domain
W Vercel dashboard → Settings → Domains → dodaj `ai-finance.pl`

## Planowane (opcja 2): migracja do Next.js + Sanity
Patrz: `../nextjs-sanity-setup/` (w przygotowaniu)
