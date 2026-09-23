# JavaScript – Service Eligibility Check

## Hjemmeopgave

I denne hjemmeopgave arbejder du videre med **JavaScript functions, conditionals og logical operators**.

Opgaven bygger videre på klasseøvelsen med `if/else`, `===`, `||`, `&&` samt forskellen på `let` og `const`.

Du arbejder selvstændigt med projektet og følger kommentarerne i filerne trin for trin.

---

# Fremgangsmåde – sådan kommer du i gang med projektet

I denne hjemmeopgave skal du bruge **GitHub Template-metoden**.

Du skal derfor **ikke downloade projektet som ZIP og ikke bruge Fork**.

Følg denne rækkefølge:

```text
GitHub Template
↓
Dit eget repository på GitHub.com
↓
GitHub Desktop
↓
Visual Studio Code
↓
Arbejd med hjemmeopgaven
↓
Commit
↓
Push
```

> Følg punkterne **ét ad gangen og i den viste rækkefølge**.

---

## 1. Opret dit eget repository på GitHub.com

Åbn det udleverede **template-repository** på GitHub.com.

Du skal være logget ind på din egen GitHub-konto.

Klik på:

**Use this template**

Vælg derefter:

**Create a new repository**

Vælg din egen GitHub-konto som ejer, og brug det repository-navn, som din underviser har angivet.

Klik derefter på:

**Create repository**

Vent et øjeblik, mens GitHub opretter dit nye repository.

### Kontrollér, at du er i dit eget repository

Når repositoryet er oprettet, skal du kontrollere navnet øverst på siden.

Det skal være **dit eget GitHub-brugernavn**, der står foran repositoryets navn.

Det kan fx se sådan ud:

```text
dit-brugernavn/js-service-eligibility-check
```

> **Stop her og kontrollér dette, før du går videre.**

---

## 2. Hent dit repository ned på din computer

Nu ligger projektet på **GitHub.com**, men du skal også have det ned på din egen computer.

Åbn **GitHub Desktop**.

Vælg:

**File → Clone repository...**

Vælg fanebladet **GitHub.com**, og find det repository, du netop har oprettet.

Hvis repositoryet ikke vises, kan du i stedet vælge fanebladet **URL** og indsætte adressen til dit repository fra GitHub.com.

### Vælg, hvor projektet skal gemmes

I feltet **Local path** vælger du, hvor projektet skal ligge på din computer.

> **Local path** betyder den mappe på din computer, hvor projektets filer bliver gemt.

Klik derefter på:

**Clone**

Vent, mens GitHub Desktop henter projektet ned på din computer.

---

## 3. Åbn projektet i Visual Studio Code

Når projektet er klonet, vælg:

**Open in Visual Studio Code**

Du skal arbejde direkte i den projektmappe, som GitHub Desktop har klonet.

Kontrollér, at projektet har denne struktur:

```text
js-service-eligibility-check/
│
├── index.html
├── js/
│   └── script.js
└── README.md
```

---

# Hjemmeopgaven

Du skal arbejde med disse filer:

- `index.html`
- `js/script.js`

Læs kommentarerne i koden grundigt, inden du begynder at skrive din løsning.

---

## 4. Forbind JavaScript-filen med HTML-filen

Åbn:

```text
index.html
```

I filen finder du denne kommentar:

```html
<!-- Husk fra dag 1: skriv scriptet, der linker til js/script.js, herunder -->
```

Din første opgave er at forbinde JavaScript-filen med HTML-dokumentet.

JavaScript-filen ligger i mappen:

```text
js/
```

og hedder:

```text
script.js
```

> **Vær opmærksom på filstien:** `script.js` ligger ikke i samme mappe som `index.html`, men i undermappen `js`.

Skriv selv det korrekte `<script>`-element på det angivne sted.

Gem derefter filen.

---

## 5. Åbn `js/script.js`

Start med at skrive:

```js
"use strict";
```

I filen finder du funktionen:

```js
tjekGratisService(brand, year)
```

Funktionen modtager to værdier:

- `brand` – bilmærket
- `year` – bilens årgang

I denne hjemmeopgave skal du arbejde videre med:

```text
if
else
===
||
&&
let
boolean
```

---

## 6. Arbejd med variablen `harGratisService`

I funktionen er denne variabel allerede oprettet:

```js
let harGratisService = false;
```

Variablen starter med værdien `false`.

Din kode skal ændre værdien til `true`, hvis bilen opfylder betingelserne for gratis service.

> Vi bruger `let`, fordi værdien kan ændres undervejs i programmet.

---

## 7. Skriv din `if/else`-struktur

Skriv selv `if/else`-strukturen inde i funktionen.

Gratis service gælder, hvis:

- bilmærket er **Volkswagen eller Skoda**
- **og** bilens årgang er større end **2023**

Hvis betingelsen er opfyldt:

- sæt `harGratisService` til `true`
- udskriv i Console, at bilen får gratis service i 1 år

Hvis betingelsen ikke er opfyldt:

- sæt `harGratisService` til `false`
- udskriv i Console, at bilen ikke får gratis service

> Brug kommentarerne i `script.js` som vejledning, men skriv selv den nødvendige JavaScript-kode.

---

## 8. Test funktionen

I `script.js` findes allerede disse funktionskald:

```js
tjekGratisService(`Volkswagen`, 2024);
tjekGratisService(`Skoda`, 2020);
tjekGratisService(`Tesla`, 2025);
```

Brug dem til at teste din løsning.

Tænk over:

- Hvilken bil opfylder hele betingelsen?
- Hvilken bil har det rigtige mærke, men en for gammel årgang?
- Hvilken bil har en ny nok årgang, men det forkerte mærke?

---

## 9. Kontrollér resultatet i browseren

Åbn `index.html` med **Live Server**.

Åbn derefter browserens Developer Tools og gå til:

```text
Inspect → Console
```

Kontrollér, at de forskellige funktionskald giver det forventede resultat.

Hvis noget ikke virker:

1. Læs eventuelle fejlmeddelelser i Console.
2. Kontrollér syntaksen.
3. Kontrollér parenteser `{ }` og `( )`.
4. Kontrollér din `if/else`-struktur.
5. Kontrollér brugen af `===`, `||` og `&&`.
6. Gem filerne og test igen.

---

## 10. Prøv forskellen på `let` og `const`

Når din løsning virker, skal du prøve følgende eksperiment:

Ret:

```js
let harGratisService = false;
```

til:

```js
const harGratisService = false;
```

Kør derefter koden igen og se, hvilken fejl du får i Console.

Overvej:

- Hvorfor opstår fejlen?
- Genkender du situationen fra klasseøvelsen?

Når du har undersøgt fejlen, skal du ændre `const` tilbage til:

```js
let
```

---

## 11. Arbejd progressivt med commits

Du skal ikke vente med at committe, til hele hjemmeopgaven er færdig.

Lav commits løbende, når du har afsluttet en tydelig del af arbejdet.

Du kan eksempelvis lave commits efter:

```text
Forbundet JavaScript med index.html
```

```text
Tilføjet use strict
```

```text
Arbejdet med servicebetingelsen
```

```text
Færdiggjort tjekGratisService-funktionen
```

```text
Testet let og const
```

Skriv selv korte og meningsfulde commit-beskeder, der beskriver, hvad du har ændret.

> Formålet er, at din Git-historik viser, hvordan du har arbejdet med hjemmeopgaven trin for trin.

---

## 12. Push til GitHub.com

Når du har lavet et commit i GitHub Desktop, skal du huske at klikke på:

**Push origin**

På den måde bliver dine ændringer sendt fra din computer til dit repository på GitHub.com.

Gå gerne ind på GitHub.com bagefter og kontrollér, at dine seneste commits kan ses.

---

# Når hjemmeopgaven er færdig

Kontrollér følgende:

- [ ] Jeg har oprettet mit eget repository med **Use this template**
- [ ] Jeg arbejder i mit eget repository
- [ ] Jeg har klonet projektet med GitHub Desktop
- [ ] Projektet er åbnet i Visual Studio Code
- [ ] `js/script.js` er forbundet korrekt med `index.html`
- [ ] Jeg har skrevet `"use strict";`
- [ ] Jeg har arbejdet med `let`
- [ ] Jeg har arbejdet med boolean-værdierne `true` og `false`
- [ ] Jeg har arbejdet med `===`
- [ ] Jeg har arbejdet med `||`
- [ ] Jeg har arbejdet med `&&`
- [ ] Jeg har færdiggjort funktionen `tjekGratisService()`
- [ ] Jeg har testet koden i browserens Console
- [ ] Jeg har undersøgt forskellen på `let` og `const`
- [ ] Jeg har lavet løbende commits
- [ ] Jeg har pushet mine commits til GitHub.com

> **Husk:** Formålet er både at træne **JavaScript functions, conditionals, logical operators og boolean-værdier** og at øve workflowet mellem **GitHub.com → GitHub Desktop → Visual Studio Code → Commit → Push**.
