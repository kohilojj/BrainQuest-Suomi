# BrainQuest Suomi

OPS-mukainen selainpeli 1.–9. luokille. 600 kysymystä (20 / oppiaine), Google-kirjautuminen, saavutukset ja leaderboard (paikallinen, valinnainen Firebase).

**Tuki:** natsaerkki@gmail.com

## Käyttöönotto
```bash
npm install
npm run dev
```
Julkaise Netlify/Vercel/GitHub Pages – ei asennuksia oppilaille.

## Google-login
GIS (Google Identity Services) käytössä. Client ID on upotettu tiedostoon `src/components/GoogleLogin.tsx`.

## Leaderboard
Oletuksena paikallinen (localStorage). Halutessasi lisää Firebasen avaimet `src/config/firebase.ts`.

## Rakenne
- `src/data/gradeX/*.json` – kysymykset aineittain ja luokittain (20 / tiedosto)
- `src/App.tsx` – sovelluksen päälogiikka (luokan/aineen valinta, peli, leaderboard)
- `src/components/*` – UI-komponentit
- `src/utils/game.ts` – pisteet yms.

Yhteensä 600 kysymystä.
