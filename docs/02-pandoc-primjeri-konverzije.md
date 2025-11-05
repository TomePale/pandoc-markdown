---
title: "Pandoc"
author: "Tome Perica"
date: "5. studenoga 2025."
lang: "hr"
---

# Pandoc - Primjeri konverzije

Pandoc je univerzalni konverter dokumenata koji omogućuje pretvaranje između različitih formata. Više informacija dostupno je na [pandoc.org](https://pandoc.org/).

## Osnovne konverzije

### Markdown → HTML

```bash
pandoc input.md -o output.html
```

**Objašnjenje:** Ova naredba pretvara Markdown datoteku (`input.md`) u HTML format (`output.html`). Pandoc automatski prepoznaje izlazni format na temelju ekstenzije datoteke.

#### Standalone HTML dokument

```bash
pandoc input.md -o output.html --standalone
```

**Objašnjenje:** Opcija `--standalone` (ili `-s`) kreira potpuni HTML dokument s `<head>` i `<body>` oznakama, umjesto samo fragmenta HTML koda.

---

### Markdown → PDF

```bash
pandoc input.md -o output.pdf
```

**Objašnjenje:** Pretvara Markdown u PDF dokument. Za ovu konverziju potreban je LaTeX (npr. TeX Live, MiKTeX ili BasicTeX).

---

### Markdown → DOCX (Microsoft Word)

```bash
pandoc input.md -o output.docx
```

**Objašnjenje:** Pretvara Markdown u Microsoft Word format (.docx), što omogućuje daljnje uređivanje u Wordu.

#### DOCX s prilagođenim predloškom

```bash
pandoc input.md -o output.docx --reference-doc=template.docx
```

**Objašnjenje:** Koristi postojeći Word dokument (`template.docx`) kao predložak za stilove (fontovi, boje, margine, itd.).

#### DOCX sa sadržajem

```bash
pandoc input.md -o output.docx --toc
```

**Objašnjenje:** Generira Word dokument s automatskim sadržajem na početku dokumenta.

---

## Dodatne korisne opcije

### Višestruki ulazni dokumenti

```bash
pandoc uvod.md poglavlje1.md poglavlje2.md -o knjiga.pdf
```

**Objašnjenje:** Spaja više Markdown datoteka u jedan izlazni dokument, što je korisno za pisanje knjiga ili dužih izvještaja.

### Specificiranje ulaznog i izlaznog formata

```bash
pandoc -f markdown -t html input.md -o output.html
```

**Objašnjenje:**
- `-f` (from) specificira ulazni format
- `-t` (to) specificira izlazni format
- Korisno kada ekstenzija datoteke nije dovoljna za automatsko prepoznavanje formata

### Konverzija s prilagođenim varijablama

```bash
pandoc input.md -o output.html --variable lang=hr
```

**Objašnjenje:** Postavlja prilagođene varijable (npr. jezik dokumenta) koje se koriste u predlošcima.



