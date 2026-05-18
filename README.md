# Crystals — Breaker Game

**Crystals** je arkadna spletna igra tipa "Brick Breaker" (uničevalec opek), zgrajena s pomočjo tehnologij HTML5 Canvas, CSS in JavaScript (z uporabo knjižnice jQuery). Igra ponuja neonsko, kristalno estetsko izkušnjo, kjer igralec z odbijanjem žogice uničuje naključno obarvane kristale.

---

## Opis naloge in delovanja

Glavni cilj igre je z uporabo drseče ploščice (paddle) obdržati žogico v igralnem polju in z njo uničiti vse kristalne opeke na vrhu zaslona. 

### Ključne funkcionalnosti:
*   **Nadzor z miško:** Igralec premika ploščico levo in desno z natančnim sledenjem premika miške. Ploščica je pomanjšana ($160\text{ px}$), kar od igralca zahteva večjo natančnost in hitrejše reflekse.
*   **Nadzorovan začetek:** Igra se ob nalaganju strani ne zažene takoj. Pripravljena je v stanju mirovanja (kjer se ploščica že odziva na miško), premikanje žogice in časovnik pa se sprožita šele ob kliku na gumb **START**.
*   **Dinamična in hitra igra:** Žogica se premika z večjo začetno hitrostjo ($dx = 3$, $dy = -5$) z osveževanjem na vsakih $5\text{ ms}$, kar zagotavlja tekočo, a hkrati zahtevno igralno izkušnjo. Kot odboja je odvisen od mesta, kjer žogica zadane ploščico.
*   **Vizualna skladnost:** Ob vsakem zagonu se generirajo naključne neonske barve kristalov. Barvna paleta žogice in ploščice je programsko usklajena z odtenki kristalov, kar ustvarja povezan retro-futurističen izgled.
*   **Sistem točkovanja in časovnik:** Vsak uničen kristal igralcu prinese $20$ točk. Stranski vmesnik sproti prikazuje trenutno število zbranih točk in čas trajanja igre v formatu `MM:SS`.
*   **Moderna zaključek igre:** Ob neuspešnem lovljenju žogice se igra zaključi. Klasično opozorilno okno je zamenjano z vizualno privlačnim in odzivnim pojavnim oknom **SweetAlert2**, ki igralcu prikaže končni čas, dosežene točke in ponudi možnost za ponovni zagon.

---

## Tehnologije

Za izdelavo projekta so bile uporabljene naslednje tehnologije:
*   **HTML5 (Canvas):** Uporabljen za izris in animacijo igralnih elementov (žogica, ploščica, opeke).
*   **CSS3:** Poskrbi za postavitev (Flexbox), neonske sence (`text-shadow`, `box-shadow`) in odzivno ozadje.
*   **JavaScript (ES6):** Logika igre, zaznavanje trkov (collision detection) in fizika odbojev.
*   **jQuery (v3.6.0):** Za enostavno manipulacijo DOM elementov in sledenje dogodkom miške.
*   **SweetAlert2:** Za napredna in stilsko oblikovana pojavna okna ob koncu igre.

---

## Navodila za zagon

1. Prenesi ali kloniraj celotno mapo s projektom.
2. Poskrbi, da imaš v mapi strukturo datotek, vključno s sliko ozadja na poti `img/ozadje.jpg`.
3. Odpri datoteko `index.html` (oziroma tvojo glavno HTML datoteko) v poljubnem sodobnem spletnem brskalniku.
4. Klikni gumb **START** v levem meniju in začni z igro.v# Kristali
