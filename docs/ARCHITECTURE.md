# Architectuur — SSPW Offerte

## Applicatie
- `index.html`: publieke zwembadcalculator.
- `admin/index.html`: beheerdashboard.
- Supabase: dynamische prijzen, leads en beheerdata.
- Vercel: hosting en deployments.
- GitHub: code en technische documentatie.

## Dataflow
Bezoeker → calculator → Supabase → resultaat / lead.

Beheerder → admin-dashboard → Supabase → prijs- en leadbeheer.

GitHub `main` → Vercel → productie.

## Branchmodel
`main` is de officiële versie. Iedere wijziging start vanaf `main` op een aparte branch en gaat via een Pull Request terug naar `main`.

## Herstelstatus 13 augustus 2026
- De rijkere en actuele code staat op `main`.
- Laatste hoofdcommit: `8ff5cce83cf725cd924b58edac028aa500f93db5`.
- De oude branch `claude/festive-rubin-k9s4ov` is geen bron van waarheid.
- De eerdere uitlegfunctionaliteit met informatie-iconen staat in `main`.
