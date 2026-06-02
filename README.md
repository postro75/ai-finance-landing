# AI & Finance — Landing Page (Production)

🌐 **Live:** https://ai-finance-landing-five.vercel.app

Statyczna strona HTML, automatyczny deploy z GitHuba przez Vercel.

## Struktura
```
.
├── index.html              # Główna strona (10 sekcji)
├── robots.txt              # SEO
├── sitemap.xml             # SEO
├── vercel.json             # Cache + security headers
├── package.json            # npm scripts
└── images/                 # Zdjęcia eksperta
    ├── expert-houndstooth.jpg   # Hero + OG image
    ├── expert-shirt.jpg         # Sekcja "O ekspercie"
    ├── expert-fullbody-gray.jpg # Rezerwa
    └── expert-portrait-id.jpg   # Favicon + logo
```

## Workflow

### Edycja treści
```bash
# Edytuj index.html
git add -A
git commit -m "Zmiana treści"
git push origin master
# Vercel auto-deploy w 30 sek
```

### Lokalne testowanie
```bash
npx serve . -l 3000
# lub
python -m http.server 3000
```

## Co trzeba uzupełnić (placeholders)

1. **Google Analytics 4** — `index.html`, szukaj `G-PLACEHOLDER`, wstaw swój Measurement ID
2. **Google Search Console** — zweryfikuj domenę w Search Console, dodaj meta tag
3. **Formularz kontaktowy** — zarejestruj się na https://formspree.io (free plan, 50/mies), wstaw endpoint ID w `index.html` (`action="https://formspree.io/f/TWOJE-ID"`)
4. **Email kontaktowy** — zamień `kontakt@ai-finance.pl` na prawdziwy adres (× 3 miejsca)
5. **Telefon** — w Schema.org JSON-LD
6. **Custom domain** (opcjonalnie) — Vercel dashboard → Settings → Domains

## Auto-deploy
- GitHub: https://github.com/postro75/ai-finance-landing
- Branch: `master`
- Każdy push = nowy deploy na production
- Preview URL przy PR

## Planowane (opcja B): Next.js + Sanity
Migracja do CMS, edycja treści przez panel. Ścieżka: `../ai-finance-next/`
