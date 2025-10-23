# Vježba 1d — Forma + slika (nadogradnja na `vjezba1c.php`)

Ova vježba nadovezuje se na **vjezba1c.php**.  
Cilj je koristiti **osnovne PHP pojmove iz uvoda** (varijable, `$_GET`, `echo`, HTML, osnovni CSS) i dodati **interakciju**:

- Forma (method **GET**) kojom student **bira temu** (dark/light),
- **Odabir slike** iz unaprijed pripremljene liste (bez uploada),
- Opcijski prikaz **opisa** (checkbox),
- Link natrag na **`vjezba1c.php`**.

> Nema naprednih koncepata (nema sesije, uploada, OOP-a).  
> Koristi samo ono što je pokriveno na uvodnom predavanju.

---

## Priprema

1. U korijenu repozitorija (ili u `/vjezba1c/`) napravi mapu **`img/`**.
2. Ubaci **tri male slike** (npr. `php.png`, `server.png`, `code.png`) — mogu biti bilo koje (slobodne ikone/slike).
3. Smjesti **`vjezba1d.php`** u isti direktorij gdje je i `vjezba1c.php`.

---

## Zadatak

1. Napravi stranicu **`vjezba1d.php`** s **PHP blokom na početku** (prije `<!DOCTYPE html>`).
2. Definiraj varijable: `$naslov`, `$autor`, `$opis` (kratka rečenica).
3. Prihvati GET parametre:
   - `tema` → `"dark"` ili `"light"` (zadano `"dark"`),
   - `slika` → `"php"`, `"server"` ili `"code"` (zadano `"php"`),
   - `opis` → checkbox (ako je postavljen, prikazati opis).
4. U HTML-u prikaži:
   - `<h1>` s naslovom,
   - rečenicu s autorom,
   - **sliku** iz mape `img/` prema izboru,
   - **opis** (ako je checkbox označen),
   - formu (method GET) s izborom teme (radio), izborom slike (select) i checkboxom za opis,
   - **dva linka/gumba**:  
     - „Primijeni odabir“ (submit forme),  
     - „Natrag na vježba 1c“.
5. Dodaj **osnovni CSS** unutar `<style>` (tamna pozadina, bijela kartica, gumb, radius, shadow).
6. Na dnu HTML-a dodaj komentar s nazivom datoteke.

---
