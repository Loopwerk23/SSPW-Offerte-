# SSPW Offerte / Zwembadcalculator

Werkende prijsindicatie-tool voor Sun Sauna & Poolworld (SSPW).

## Status
- Officiële codebasis: `main`
- Productiehosting: Vercel
- Data, prijzen, leads en authenticatie: Supabase
- Calculator: `index.html`
- Beheerdashboard: `admin/index.html`

## Belangrijk
De branch `claude/festive-rubin-k9s4ov` is een oude ontwikkelbranch en is **niet** de leidende versie. Nieuwe werkzaamheden starten altijd vanaf `main` op een aparte feature/agent-branch en gaan via een Pull Request terug naar `main`.

## Huidige functionaliteit
- prijsindicatie voor standaard- en maatwerkzwembaden;
- prijzen en instellingen laden uit Supabase met fallback;
- lead capture en opslag;
- admin-dashboard voor leads en prijsbeheer;
- rollen voor beheerders;
- CSV/Excel-export van leads;
- uitleg-informatie via `i`-iconen bij maten, pakketonderdelen en opties;
- Vercel Analytics en Speed Insights.

## Documentatie
- `docs/ARCHITECTURE.md` — technische opbouw en bron van waarheid.
- `docs/SOP-001-GitHub-Branchbeheer.md` — vaste werkwijze voor wijzigingen.
- `docs/PLAN.md` — oorspronkelijke ontwikkelplanning; kan historische informatie bevatten.
- `CLAUDE.md` — instructies voor AI-ontwikkelaars.

## Werkregel
**Nooit direct op `main` ontwikkelen.** Maak een branch, test de wijziging, open een Pull Request en merge pas daarna naar `main`.
