# AI Development Instructions — SSPW Offerte

Deze instructies gelden voor Claude, ChatGPT/Codex en andere AI-ontwikkelaars die aan deze repository werken.

## Bron van waarheid
- `main` is de officiële, stabiele versie.
- Supabase is de bron voor live prijzen, leads, gebruikers en rollen.
- Vercel publiceert de applicatie.
- `docs/` bevat architectuur en SOP's.

## Verplichte werkwijze
1. Lees eerst `README.md`, `docs/ARCHITECTURE.md` en relevante SOP's.
2. Start nooit direct op `main`.
3. Maak voor iedere wijziging een aparte branch vanaf de actuele `main`.
4. Behoud bestaande functionaliteit tenzij expliciet anders gevraagd.
5. Test de volledige gebruikersflow vóór merge.
6. Open een Pull Request naar `main` met een duidelijke beschrijving.
7. Werk documentatie bij wanneer architectuur, dataflow of beheer verandert.

## Nooit zonder expliciete toestemming
- productiedata verwijderen;
- Supabase-tabellen, RLS-regels, rollen of authenticatie ingrijpend wijzigen;
- secrets/API-keys committen;
- productieconfiguratie of domeinen wijzigen;
- bestaande werkende functionaliteit herschrijven alleen om code 'netter' te maken;
- branches of historische commits verwijderen.

## Functionele aandachtspunten
- De tool geeft een indicatieve prijs, geen bindende offerte.
- De volledige prijsindicatie volgt na lead capture.
- Prijzen worden primair uit Supabase geladen; ingebouwde waarden vormen fallback.
- Uitlegvelden (`info`) bij maten, pakketonderdelen, groepen en opties moeten behouden blijven.
- Adminrollen en toegangsbeveiliging moeten behouden blijven.

## Definition of done
Een wijziging is pas klaar wanneer:
- de calculatorflow werkt;
- relevante admin-functionaliteit werkt;
- geen consolefouten optreden in de aangepaste flow;
- Supabase-fallback niet is gebroken;
- de wijziging in een Pull Request staat;
- relevante SOP/documentatie is bijgewerkt.
