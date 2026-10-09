# Task Manager

Task Manager er en enkel oppgaveliste. Skriv inn en oppgave for å legge den til, marker den som fullført når du er ferdig, eller slett den. Oppgavene lagres i nettleseren slik at de fortsatt vises neste gang du åpner nettsiden.

## Hva Task Manager gjør
Task Manager samler oppgaver i en liste og lar brukeren holde oversikt over hva som er gjort og hva som gjenstår.

## Hvilke teknologier jeg har brukt
- HTML for struktur og innhold
- CSS for styling og layout
- JavaScript for funksjonalitet og interaktivitet
- localStorage for å lagre oppgavene i nettleseren

## Hvordan man starter nettsiden

På VSC:
1. Gå til prosjektmappen `task-manager`.
2. Åpne filen `index.html` med "show preview" eller "go live"

På GitHub:
1. Klikk på eller søk denne lenken: ""


## Hvilke funksjoner som er implementert
- Legge til oppgaver med knappen eller Enter
- Markere oppgaver som fullført
- Slette oppgaver
- Lagre oppgaver og fullføringsstatus i localStorage
- Laste inn de lagrede oppgavene når siden åpnes på nytt
- Vise oppgavene i en liste

## Hvilke tester jeg har gjennomført
Jeg har testet følgende manuelt i nettleseren:
- At en oppgave kan legges til med knappen
- At en oppgave kan legges til ved å trykke Enter
- At en oppgave vises i listen etter at den er lagt til
- At en oppgave kan markeres som fullført
- At en oppgave kan slettes
- At oppgaver som er lagret, fortsatt vises etter at siden lastes inn på nytt

## Hvilke feil jeg fant, og hvordan jeg rettet dem

1. Det var ikke et fungerende felt for å skrive inn oppgaver.
   - Årsak: feltet var satt opp som et e-postfelt, selv om det skulle ta imot oppgavetekst.
   - Løsning: feltet ble endret til et tekstfelt for oppgaver.

2. Oppgaver ble ikke lagt til og vist i en liste.
   - Årsak: JavaScript-funksjonaliteten for å opprette listeelementer og håndtere knappetrykk manglet.
   - Løsning: jeg la til funksjonalitet som oppretter og viser oppgaver, og som også støtter Enter.

3. Oppgaver ble ikke beholdt etter at siden ble lukket eller lastet inn på nytt.
   - Årsak: oppgavelisten ble ikke lagret.
   - Løsning: jeg la til lagring og innlasting med localStorage. Fullføringsstatus lagres også.
