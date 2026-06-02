# Atelje 138 — uputstvo (sajt, slike, forme, hosting)

## 1. Šta je u paketu
- `index.html` — ceo sajt u jednom fajlu (SR, sa prevodom EN/RU u gornjem desnom uglu).
- Folder `images/` — ovde ideš tvoje fotografije za galeriju (vidi tačku 2).

Dizajn: tirkizna + roze + ljubičasta, naslovi font **Fraunces**. Sve sekcije: Hero, O ateljeu, Radionice (dugme **ZA DECU / ZA ODRASLE**), Poklon vaučer, Galerija, Kontakt + mapa.

## 2. Galerija — dodaj svoje slike
Sajt traži 12 slika iz foldera `images` sa imenima `g1.jpg`, `g2.jpg` … `g12.jpg`.
1. Napravi folder `images` pored `index.html`.
2. Preimenuj svoje fotografije u `g1.jpg`, `g2.jpg` … `g12.jpg` i ubaci ih unutra.
3. Ako neka slika fali, na njenom mestu se prikaže lepa ikonica — sajt se neće „polomiti".

> Slike koje si poslao u chatu nisu mi dostupne kao fajlovi, pa ih ti ubaci na ovaj način. Preporuka: kvadratne ili pejzaž, do ~1600px, optimizovane (manje od 500 KB svaka) zbog brzine.

## 3. Forme idu na tvoj e-mail (atelje138@gmail.com)
Obe forme (prijava za radionicu i zahtev za poklon vaučer) koriste **FormSubmit** — besplatno, bez naloga.
- **Prvi put** kada neko pošalje formu, FormSubmit ti šalje mejl sa dugmetom **„Activate"** — klikni ga jednom da potvrdiš adresu. Posle toga sve prijave stižu automatski na atelje138@gmail.com.
- Ništa ne moraš da menjaš u kodu — adresa je već upisana.

## 4. Besplatan hosting — Netlify (najlakše, drag & drop)
1. Idi na **netlify.com** → **Sign up** (može preko Google naloga atelje138@gmail.com).
2. Na dashboard-u izaberi **Add new site → Deploy manually**.
3. **Prevuci ceo folder** (sa `index.html` i folderom `images`) u polje za otpremanje.
4. Za par sekundi dobiješ adresu tipa `nasumicno-ime.netlify.app`. Sajt je živ.
5. Promeni ime: **Site configuration → Change site name** → npr. `atelje138`.
6. Kad menjaš nešto kasnije: opet prevučeš folder na isto mesto (Deploys → Drag and drop).

## 5. Povezivanje domena `atelje138.rs`
1. Kupi domen `.rs` kod registra (npr. **mCloud / Loopia / Plus hosting / Beotel** — RNIDS registrari). Cena ~1.500–2.500 RSD/god.
2. U Netlify: **Domain management → Add a domain** → upiši `atelje138.rs`.
3. Netlify ti da DNS podatke. Dve opcije:
   - **Lakše:** kod registrara podesi **nameservers** na Netlify-jeve (`dns1.p0X.nsone.net` …) — Netlify ih prikaže.
   - **Ili:** dodaj zapise ručno kod registrara:
     - `A` zapis: `@` → `75.2.60.5`
     - `CNAME`: `www` → `tvoje-ime.netlify.app`
4. Sačekaj da se DNS propagira (od par minuta do 24h). Netlify automatski uključi **besplatni HTTPS (SSL)**.

## 6. Alternativa — GitHub Pages (besplatno, bez vremenskog ograničenja)
1. Napravi nalog na **github.com**.
2. **New repository** → ime `atelje138` → Public.
3. **Add file → Upload files** → prevuci `index.html` i folder `images` → Commit.
4. **Settings → Pages → Source: Deploy from branch → main /(root) → Save.**
5. Posle minut sajt je na `https://tvoj-nalog.github.io/atelje138/`.
6. Za domen `atelje138.rs`: **Settings → Pages → Custom domain** → upiši domen; kod registrara dodaj `A` zapise ka GitHub IP (`185.199.108.153`, `.109.153`, `.110.153`, `.111.153`) i `CNAME www → tvoj-nalog.github.io`.

## 7. Sledeći koraci (predlozi)
- **Plaćanje vaučera onlajn:** trenutno forma šalje zahtev na mejl, a plaćanje se dogovara ručno. Ako želiš pravo onlajn plaćanje karticom, mogu da dodam dugme preko domaćeg provajdera (npr. AllSecure/WSPay/banka) ili PayPal — to traži otvaranje naloga kod provajdera.
- **Google Business profil:** da se mapa i recenzije bolje prikazuju — mogu da ti napišem optimizovan opis.
- **Cenovnik PDF:** mogu da napravim lep štampani cenovnik/flajer u istom dizajnu.
- **Više jezika u meta podacima** (SEO) za bolju vidljivost na pretrazi.

Reci samo šta od ovoga da uradim sledeće.
