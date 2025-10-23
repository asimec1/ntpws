# Vježba 1c — PHP dokument (nastavak na vjezba1b.php)

Ova vježba je nastavak prethodne **vjezbe1b.php** i služi za ponavljanje PHP pojmova:
- PHP blok na početku dokumenta  
- Varijable i ispis pomoću `echo`  
- HTML struktura i osnovni CSS  
- Dodavanje linkova i meta podataka

Cilj je naučiti kako PHP i HTML zajedno tvore dinamičnu web stranicu.

---

## Zadatak

1. Kreiraj datoteku `vjezba1c.php` u istoj mapi kao `vjezba1b.php`.
2. PHP blok mora biti **na početku datoteke**, prije `<!DOCTYPE html>`.
3. U PHP dijelu definiraj varijable:
   - `$naslov` – naslov stranice (npr. "PHP dokument — vježba 1c")
   - `$autor` – tvoje ime i prezime
   - `$opis` – kratki opis stranice (jedna rečenica)
   - `$linkInfo` – vanjski URL (npr. https://www.php.net)
   - `$linkNatrag` – relativni link koji vodi na **vjezba1b.php**
4. U HTML dijelu prikaži:
   - `<h1>` s naslovom
   - Dva odlomka s opisom i imenom autora
   - Dva linka:
     - **„Saznaj više o PHP-u“** (otvara se u novoj kartici)
     - **„Natrag na vježba 1b“** (vodi na prethodnu stranicu)
   - Podnožje s trenutnom godinom (`date('Y')`)
5. Dodaj **osnovni CSS** unutar `<style>`:
   - tamna pozadina stranice (`--bg`)
   - bijela kartica s tekstom (`--card`)
   - zaobljeni rubovi i blagi shadow
   - gumb-link s hover efektom
6. Na dnu HTML-a dodaj komentar s nazivom datoteke.

---

