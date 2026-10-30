# Startside

En enkel startside for nettleseren med egne lenker, frister, været for Slemmestad fra Yr og gule lapper. Hver person fyller den med sitt eget innhold, så flere kan bruke samme adresse.

## Publisere på GitHub Pages

1. Lag et nytt repo på GitHub, for eksempel `startside`.
2. Last opp `index.html` og `README.md`. Filen må hete nøyaktig `index.html`.
3. Gå til **Settings → Pages**, velg **Deploy from a branch**, branch `main` og mappe `/ (root)`, og trykk **Save**.
4. Etter et minutt eller to ligger siden på `https://<brukernavn>.github.io/startside/`.

Når du laster opp en ny versjon: vent til jobben under **Actions** er grønn, og trykk **Ctrl + F5** på startsiden.

### Ny versjon med annet filnavn

Nye versjoner kommer som `startside.html`, så de ikke blandes med andre `index.html`-filer i Nedlastinger. GitHub Pages viser bare filen som heter `index.html`, så innholdet må inn i den. Enklest:

1. Åpne `startside.html` i Notisblokk, merk alt (Ctrl + A) og kopier.
2. Åpne `index.html` i repoet på GitHub og trykk blyanten (**Edit this file**).
3. Merk alt i redigeringsfeltet, lim inn og trykk **Commit changes**.

## Sette den som startside i Edge

1. Åpne `edge://settings/startHomeNewTab`.
2. Under **Når Edge starter** velger du **Åpne disse sidene** og legger inn adressen fra GitHub Pages.
3. Vil du også ha en hjem-knapp, slår du på **Vis Hjem-knappen på verktøylinjen** under **Hjem-knapp** og limer inn samme adresse.

Edge lar deg ikke bytte ut siden som vises i en ny fane uten en utvidelse.

## Lenker

- **Dra inn:** Dra ikonet til venstre i adressefeltet (eller en lenke fra en annen side) og slipp det på startsiden.
- **Legg til manuelt:** Trykk på ruta med pluss og lim inn adressen. Det er nyttig på mobil.
- **Endre eller fjerne:** Hold musepekeren over en lenke og trykk ✎ for nytt navn eller × for å fjerne den.

Ikonet hentes automatisk fra nettstedet. Sider uten eget ikon får en farget rute med forbokstaven. Noen jobbsider har faste ikoner, og de står i lista `KNOWN_ICONS` i `index.html`.

## Frister

Skriv inn tittel og dato til venstre. Fristene sorteres med den nærmeste øverst. Under to uker igjen blir de oransje, og passerte frister blir røde.

## Handlelista

Handlelista hentes fra den samme Firebase-databasen som Handlelista-appen, så endringer vises med en gang begge steder.

- Første gang limer du inn delingslenken fra appen (knappen **Del**) og trykker **Koble til**.
- Skriv en vare og trykk Enter. Tall først gir antall («2 melk»), og komma legger til flere på én gang.
- Trykk på en vare for å krysse den av. Redigering og sletting gjør du i appen.
- Listekoden står ikke i koden på GitHub. Den lagres bare i nettleseren, og den er med i sikkerhetskopien.

## Lagring og sikkerhetskopi

Lenker, frister og lapper lagres i nettleseren på den maskinen du bruker. De følger ikke med til andre maskiner eller nettlesere, og de forsvinner hvis du sletter nettleserdata for siden.

Nederst på siden ligger to knapper:

- **Lagre sikkerhetskopi** laster ned alt som en fil.
- **Hent sikkerhetskopi** leser filen inn igjen og erstatter det som ligger på siden. Bruk den når du bytter PC eller nettleser.

## Endre vær-modulen

Yr-modulen er en `iframe` i `index.html`. Vil du ha et annet sted, kan du lage ny kode på yr.no/nb/widget og lime den inn i stedet.
