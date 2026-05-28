# Teknisk dokumentation - Grp. 6

---

## Om Projekt

I dette projekt har vi lavet et redesign af Sidecars hjemmeside. Vi har udviklet sitet med astro. I implementeringen har vi brugt HTML, CSS og javascript til opbygning og styling af projektet.

---

## Team medlemmer

- Ea (cocktailcatering.astro + cocktailmenu.astro + Footer.astro)
- Iben (selskaber.astro + [id].astro + Pakke.astro + Enkelpakke.astro)
- Laura (menukort.astro + tilhørende komponenter fx. Menumad.astro)
- Sofie (index.astro + Header.astro)

---

### Links

- GitHub repository: https://github.com/ibenlehmann/sidecar 
- Figma: https://www.figma.com/design/Mztrq6JaJUudSdbim1fl2Z/Eksamen---gruppe-6?node-id=0-1&t=OJnpYJvMA5ymv60Q-1
- Trello: https://trello.com/b/5IpqWraj/eksamensprojekt-team-6

---

## Projektstruktur

```
project/
├── public/
│   ├── favicon.ico
│   ├── favicon.svg
│   └── img/
├── src/
│   ├── components/
│   │   ├── Beer.astro
│   │   ├── Brunchdrinks.astro
│   │   ├── Coffee.astro
│   │   ├── Colddrinks.astro
│   │   ├── Enkelpakke.astro
│   │   ├── Footer.astro
│   │   ├── Header.astro
│   │   ├── Matcha.astro
│   │   ├── Menumad.astro
│   │   ├── Other.astro
│   │   ├── Pakke.astro
│   │   ├── Tea.astro
│   │   └── Wine.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   ├── enkel_pakke/
│   │   │   └── [id].astro
│   │   ├── cocktailcatering.astro
│   │   ├── cocktailmenu.astro
│   │   ├── index.astro
│   │   ├── menukort.astro
│   │   └── selskaber.astro
├── .env
└── README.md
```

---

## Filbeskrivelser

- index.astro – Forsiden
- menu.astro – viser en liste med data fra API'et, hvor der hentes flere tabeller, til at lave menu cards
- Menumad.astro - komponent, som kalder på props, og styling af cards
- selskaber.astro – viser en liste med data fra API'et, hvor der hentes en tabel, til at lave pakke cards
- [id].astro - viser individuelle id'er fra API'et
- cocktailcatering.astro - indeholder formular
- cocktailmenu.astro - statisk side
- Layout.astro ─ styrer hovedlayoutet for alle sider og global style
- Footer.astro & Header.astro - komponenter, der bruges til navigationbaren og til sidens footer

---

# Data og JSON-struktur

Igennem supabase henter vi data fra et API i JSON-format.

#### To af vores objekter ser fx sådan ud:

```
[
  {
    "id": 1,
    "created_at": "2026-05-18T08:58:27.144324+00:00",
    "nummer": "Pakke 1",
    "navn": "Frokostarrangement",
    "info": "  Pakken til dit næste frokostarrangement\n  \u003Cul\u003E\n\u003Cli\u003EFlere frokostretter end de klassiske brunchretter \n\u003Cli\u003ELokaleleje fra kl. 13-16 med fuld forplejning\n\u003Cli\u003E319kr per kuvert \n\u003Cli\u003E159kr for børn fra 3-12 \n\u003Cli\u003E3999kr i lokaleleje\n\u003C/ul\u003E",
    "img": "https://qvojbjzhnzwsmxjbsnze.supabase.co/storage/v1/object/public/pakke_img/pakke1.webp"
  },
]

[
    {
    "id": 1,
    "created_at": "2026-05-18T09:05:22.400692+00:00",
    "navn": "Scrambled eggs",
    "beskrivelse": "with lactose free cream & chives "
  },
]
```

---

# Felter vi bruger

pakke
- nummer - pakke nummer
- navn - navn på pakke
- info - info om pakke
- img - billede

menumad
- name - navn på mad
- beskrivelse - mere info om mad
- pris - pris i kr.

## Navngivning

Vi har prøvet at navngive vores filer, variabler og funktioner så tydeligt som muligt.

Eks.
cocktailcatering.astro - er siden om cocktail catering

---

## Git og Branches

Vi har brugt Github til at samarbejde om projektet.

Vi arbejder i branches, så vi ikke ændre i det samme samtidig

### Workflow

1. Lave en branch med et beskrivende feature-navn eller med eget navn
2. Kode en feature
3. Committe ændringer
4. Pushe til GitHub
5. Merge til main

---

## Bæredygtighed

Vi kodede siden i Astro, da det bidrager til at gøre den mere bæredygtig. Dette skyldes, at kodningen er komponentbaseret, så vi på denne måde har genbrugt vores elementer flere steder. Derved undgår man unødvendige loading, da der ikke er for mange gentagelser af kode.

Derudover har vi brugt WebP-format til alle vores billeder, som optimerer filstørrelsen på billederne og derfor også giver mindre loadtid, når brugerne besøger sitet. Billederne er stadig i høj kvalitet, men filstørrelsen er komprimeret med omkring 25%, så filerne er lettere, hvilket også er godt for søgemaskineoptimering. 

## Udfordringer undervejs

Vi har haft nogle forskellige små udfordringer undervejs, som vi har løst i fællesskab.

## Mulige forbedringer

- Mere overskuelig menukort
- Mindre tekst
- Generelt alt mindre 

---

## Gruppemedlemmer:

- Ea Lotz
- Iben Lehmann
- Laura Buschardt
- Sofie Høgh-Olesen
