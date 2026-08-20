# Landingpage-Brugermanualtilditbarn.dk

Invitation og tilmeldingsside til Manual-receptionen den 1. september 2026.

Almindelig, statisk hjemmeside — én fil (`index.html`), intet build-trin, ingen database.
Tilmeldinger opsamles automatisk af Netlify (Netlify Forms), og dukker op under
**Site configuration → Forms** i Netlify-dashboardet, med mulighed for at slå
e-mailnotifikation til pr. tilmelding.

## Sådan får I siden i luften

1. Gå til [netlify.com](https://www.netlify.com) og opret en gratis konto (eller log ind).
2. Vælg **Add new site → Import an existing project** og forbind jeres GitHub-konto.
3. Vælg dette repository (`Landingpage-Brugermanualtilditbarn.dk`).
4. Byggeindstillinger skal ikke ændres — der er ingen build command og publish directory er `.` (roden). Klik **Deploy**.
5. Når sitet er deployet, får I en `*.netlify.app`-adresse. Gå til **Domain settings** og tilføj jeres eget domæne `brugermanualtilditbarn.dk`.
6. Følg Netlifys vejledning for at pege domænet herhen — det gøres ved at ændre DNS/nameservers hos Simply.com. Sig til hvis I vil have hjælp til det skridt.
7. Under **Site configuration → Forms** kan I slå en e-mail-notifikation til, så I får en mail for hver tilmelding.

## Redigere indhold

Alt tekst og alle links ligger i `index.html`. Det er en almindelig tekstfil —
I kan redigere den direkte på GitHub.com (åbn filen, tryk på blyant-ikonet,
gem som en "commit") uden at installere noget. Netlify bygger siden igen automatisk
efter hvert gem.

## Billede

`images/invitation.png` er selve invitationsgrafikken. Klikbare områder (bog,
Momenta-logo, bamse/tilmeld) er lagt ovenpå billedet som usynlige felter placeret
med procent-koordinater i `<style>`-blokken i `index.html`. Skiftes billedet ud
med et andet layout, skal disse koordinater justeres.
