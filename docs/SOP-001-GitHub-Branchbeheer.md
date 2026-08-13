# SOP-001 — GitHub branchbeheer

## Doel
De werkende SSPW-tool veilig houden terwijl er wijzigingen worden gedaan.

## Werkwijze
1. Start altijd vanaf `main`.
2. Maak een aparte branch voor de wijziging.
3. Voer alleen de bedoelde wijziging uit.
4. Test de calculator en relevante beheerfuncties.
5. Open een Pull Request met `main` als doelbranch.
6. Controleer de wijziging.
7. Merge pas na akkoord naar `main`.
8. Controleer daarna de live versie.
9. Werk documentatie bij wanneer de werkwijze verandert.

## Branchnamen
- `agent/...` voor AI-ondersteunde wijzigingen.
- `feature/...` voor nieuwe functionaliteit.
- `fix/...` voor herstelwerk.

## Afspraken
- `main` is de officiële versie.
- De oude Claude-branch is geen doelbranch.
- Oude branches blijven voorlopig bestaan als herstelreferentie.
- Structurele wijzigingen worden ook in de documentatie vastgelegd.

## Herstel bij fouten
1. Stop verdere merges.
2. Bepaal de laatste werkende commit op `main`.
3. Zoek welke wijziging het probleem veroorzaakte.
4. Herstel via een aparte fix-branch.
5. Test opnieuw vóór de volgende merge.
