# Upute za CSS (obavezno)

Ovo su pravila koja studenti trebaju ispoštovati za **Vjezba1b**.  
Ne moraju biti 100 % ista imena varijabli ili klasa, ali **vizual i ponašanje moraju odgovarati**.

---

## 1) Struktura i organizacija

- CSS smjestiti **unutar `<style>` u `<head>`** (nema zasebne `.css` datoteke).
- Na početku definirati **CSS varijable** u `:root`.
- Koristiti **jednostavne klase** bez dubokog ugnježđivanja.

---

## 2) Boje i kontrast

- Definirati u `:root`:
  - `--bg` → tamna pozadina stranice  
  - `--card` → bijeli sadržajni blok  
  - `--text` → tamni tekst  
  - `--muted` → sivi sekundarni tekst  
  - `--accent` → primarna boja za naglaske i gumb  
- Tekst mora imati **dovoljan kontrast** (npr. tamno na svijetlom ili obratno, WCAG AA).

---

## 3) Tipografija

- Osnovni font:  
  `system-ui, -apple-system, "Segoe UI", Roboto, sans-serif`
- Bazna veličina: **16 px**  
- Naslov `<h1>`: **najmanje 2 rem**  
- **Line-height**: oko **1.6** za ugodno čitanje paragrafa

---

## 4) Layout (kontejner “kartica”)

- Glavni kontejner (npr. `.wrap`):
  - `max-width: 720px`
  - `margin: 48px auto`
  - `background: var(--card)`
  - `padding: 32px`
  - `border-radius: 16px`
  - `box-shadow: 0 10px 30px rgba(0,0,0,.08)`
- Tijelo stranice (`body`):
  - `margin: 0`
  - `background: var(--bg)`
  - `color: var(--text)`
  - Globalni `box-sizing: border-box`

---

## 5) Elementi teksta

- `<h1>`:
  - bez gornjeg margina
  - donji margin 12–16 px  
- `<p>`:
  - donji margin 12–16 px
  - line-height ~1.6  
- Sekundarni tekst (npr. `footer`):
  - manji font (≈ 0.9 rem)
  - `color: var(--muted)`

---

## 6) Gumb / link (primarna radnja)

- Klasa `.btn` (na `<a>`):
  - `display: inline-block`
  - `padding: 10px 16px`
  - `border: 1px solid var(--accent)`
  - `border-radius: 10px`
  - `text-decoration: none`
- Stanja:
  - `:hover` → `background: var(--accent); color: #fff`
  - `:focus-visible` → `outline: 3px solid var(--accent)`
  - `:active` → blago zatamnjenje (manji opacity)
- Obični link (koji nije gumb) neka ima normalnu boju teksta, bez podcrtavanja osim na hoveru.

---

## 7) Responsivnost

- Stranica mora biti **čitljiva na mobitelu**:
  - `<meta name="viewport" ...>` već postoji
  - `.wrap` zauzima 100 % širine do max 720 px
  - Tekst ostaje čitljiv, bez horizontalnog scrolla  
- Nije potreban grid ili flex layout osim za poravnanje gumba.

---

## 8) Animacije i pristupačnost

- Ako se koristi tranzicija:  
  **0.15 – 0.2 s**, suptilno i bez treperenja  
- Poštovati `prefers-reduced-motion` (ako se koristi)  
- Fokus s tipkovnice mora biti **vidljiv** (outline ili border)

---

## 9) Kod stil

- Ujednačeni razmaci i uvlake (2 ili 4 razmaka)
- Imena klasa kratka i smislenа (`.wrap`, `.btn`)
- Izbjegavati `!important` osim u krajnjoj nuždi (ovdje nije potrebno)

---

