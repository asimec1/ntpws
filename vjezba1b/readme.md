# ntpws
Upute za CSS (obavezno)
1) Struktura i organizacija
	CSS smjestiti u <style> unutar <head> (za ovaj zadatak nema zasebne .css datoteke).
	Na početku definirati CSS varijable (boje) u :root.
	Koristiti jednostavne klase (bez prekomjernog ugnježđivanja).

2) Boje i kontrast
	Definirati u :root:
		--bg (tamna pozadina stranice),
		--card (bijeli sadržajni blok),
		--text (tamni tekst),
		--muted (sekundarni/sivi tekst),
		--accent (primarna naglasna boja – isti ton za obrub gumba i hover).
	Tekst na pozadini mora imati dobar kontrast (ciljati WCAG AA, npr. crna/tamna na bijelom i obratno).

3) Tipografija
	Osnovni font: system-ui, -apple-system, "Segoe UI", Roboto, sans-serif.
	Bazna veličina: 16px (browser default).
	Naslov <h1>: min 2rem; standardni odmak ispod.
	Line-height ~1.6 za paragraf.

4) Layout (kontejner “kartica”)
	Središnji kontejner (klasa npr. .wrap):
		max-width: 720px,
		margin: 48px auto,
		background: var(--card),
		padding: 32px,
		border-radius: 16px,
		lagani shadow (box-shadow) za odvojenost od pozadine.
	Tijelo stranice (body):
		margin: 0,
		background: var(--bg),
		color: var(--text),
		box-sizing: border-box globalno (* { box-sizing: border-box; }).

5) Elementi teksta
	<h1>:
		bez gornjeg margina, donji margin ~12–16px.
	<p>:
		donji margin 12–16px,
		standardni line-height (vidi Tipografija).
		Sekundarni tekst (npr. footer):
		manji font (≈0.9rem),
		muted boja: color: var(--muted).

6) Dugme / link (primarna radnja)
	Klasa npr. .btn (koristi se na <a>):
		display: inline-block,
		padding ≈ 10px 16px,
		border: 1px solid var(--accent),
		border-radius: ≈ 10px,
		**text-decoration: none`.
	Stanja:
		:hover → background: var(--accent); color: #fff;
		:focus-visible → jasan outline (npr. outline: 3px solid var(--accent)),
		:active → lagano zatamnjenje (smanjen opacity ili tamnija nijansa).
	Link koji nije gumb neka nasljeđuje boju teksta; bez podcrtavanja dok nije hover (po izboru).

7) Responsivnost
	Stranica mora biti čitljiva na mobitelu:
		meta viewport već je u HTML-u,
		kontejner .wrap zauzima 100% širine do max 720px,
		tipografija i margine ostaju čitljive.

8) Animacije i pristupačnost
	Ako se koristi tranzicija, neka bude suptilna (0.15–0.2s) i neovisna o pokretima.
	Poštovati prefers-reduced-motion (ako ga koristite – nije obavezno).
	Fokus (keyboard) mora biti vidljiv na gumbu/linku.

9) Kod stil
	Ujednačeni razmaci i uvlake (2 ili 4 razmaka).
	Imena klasa kratka i smislenа (.wrap, .btn).
	Ne koristiti !important osim ako baš morate.
