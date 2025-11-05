---
title: "Markdown - Primjeri sintakse"
author: "Tome Perica"
date: "5. studenoga 2025."
lang: "hr"
---

# Markdown - Primjeri sintakse

Ovaj dokument prikazuje osnovne elemente Markdown sintakse prema [GitHub vodiču za Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

## Naslovi

Naslovi se kreiraju pomoću `#` simbola. Broj `#` znakova određuje razinu naslova:

# Naslov prve razine (H1)
## Naslov druge razine (H2)
### Naslov treće razine (H3)
#### Naslov četvrte razine (H4)
##### Naslov pete razine (H5)
###### Naslov šeste razine (H6)

---

## Liste

### Nenumerirana lista

Nenumerirane liste koriste `-`, `*` ili `+` simbole:

- Prva stavka
- Druga stavka
- Treća stavka
  - Podstavka 1
  - Podstavka 2
    - Pod-podstavka

### Numerirana lista

Numerirane liste koriste brojeve s točkom:

1. Prvi korak
2. Drugi korak
3. Treći korak
   1. Podkorak 3.1
   2. Podkorak 3.2
4. Četvrti korak

### Mješovita lista

Možete kombinirati numerirane i nenumerirane liste:

1. Glavni zadatak
   - Podzadatak A
   - Podzadatak B
2. Drugi glavni zadatak
   - Podzadatak C

---

## Tablica

Tablice se kreiraju pomoću vertikalnih crta `|` i crtice `-`:

| Naziv | Tip | Veličina | Opis |
|-------|-----|----------|------|
| CHANGELOG.md | Markdown | 2 KB | Dokumentacija projekta |
| script.js | JavaScript | 5 KB | Glavni skript |
| config.json | JSON | 1 KB | Konfiguracijska datoteka |
| index.html | HTML | 3 KB | Početna stranica |

### Poravnanje u tablicama

Možete kontrolirati poravnanje teksta u stupcima:

| Lijevo poravnano | Centrirano | Desno poravnano |
|:-----------------|:----------:|----------------:|
| Tekst | Tekst | Tekst |
| 100 | 200 | 300 |
| A | B | C |

---

## Slike

Slike se umeću pomoću sintakse: `![alt tekst](putanja/do/slike.png)`

### Primjer slike

![Tux - Linux maskota](../static/base-octocat.svg)

*Slika: Octocat, službena maskota GitHuba*

---

## Blokovi koda

### Inline kod

Inline kod se piše između jednostrukih `` ` `` znakova: `print("Hello, World!")`.

### Code block (bash)

```bash
# Provjera verzije
pandoc --version
```

### Code block (JavaScript)

```javascript
// Primjer JavaScript koda
function izracunaj(a, b) {
    return a + b;
}

const rezultat = izracunaj(5, 10);
console.log(`Rezultat: ${rezultat}`);
```

---

## Poveznice

### Vanjska poveznica

Za više informacija o Markdownu posjetite [GitHub Docs](https://docs.github.com/en/get-started/writing-on-github).

### Poveznica s opisom

Više o Pandocu možete saznati na [službenoj Pandoc stranici](https://pandoc.org/).

### Poveznica na lokalnu datoteku

Pogledajte [primjere konverzije s Pandocom](02-pandoc-primjeri-konverzije.md).

---

## Dodatne mogućnosti

### Isticanje teksta

- **Podebljano** ili __podebljano__
- *Kurziv* ili _kurziv_
- ***Podebljano i kurziv***
- ~~Precrtano~~

### Citati

> Ovo je citat.
>
> Može se protezati kroz više redaka.
>
> — Autor

### Horizontalna linija

Koristi se `---`, `***` ili `___`:

---

### Zadaci (Task list)

- [x] Napisati dokumentaciju
- [x] Dodati primjere
- [x] Testirati konverziju u PDF
- [x] Objaviti projekt


