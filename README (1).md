# Startside

En enkel startside for nettleseren med store lenkeikoner, været for Slemmestad fra Yr og gule lapper.

## Publisere på GitHub Pages

1. Lag et nytt repo på GitHub, for eksempel `startside`.
2. Last opp `index.html` og `README.md`. Filen må hete nøyaktig `index.html`.
3. Gå til **Settings → Pages**, velg **Deploy from a branch**, branch `main` og mappe `/ (root)`, og trykk **Save**.
4. Etter et minutt eller to ligger siden på `https://<brukernavn>.github.io/startside/`.

## Sette den som startside i Edge

1. Åpne `edge://settings/startHomeNewTab`.
2. Under **Når Edge starter** velger du **Åpne disse sidene** og legger inn adressen fra GitHub Pages.
3. Vil du også ha en hjem-knapp, slår du på **Vis Hjem-knappen på verktøylinjen** under **Hjem-knapp** og limer inn samme adresse.

Edge lar deg ikke bytte ut siden som vises i en ny fane uten en utvidelse.

## Endre lenker

Øverst i `<script>`-delen i `index.html` ligger en liste som heter `LINKS`. Legg til, fjern eller flytt linjer der. Ikonene hentes automatisk.

## Om lappene

Lappene lagres i Edge på den PC-en du bruker. De følger ikke med til andre maskiner eller nettlesere, og de forsvinner hvis du sletter nettleserdata for siden.

## Endre vær-modulen

Yr-modulen er en `iframe` i `index.html`. Vil du ha en annen modul eller et annet sted, kan du lage ny kode på yr.no/nb/widget og lime den inn i stedet.
