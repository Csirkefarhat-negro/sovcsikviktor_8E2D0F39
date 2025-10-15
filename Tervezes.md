### Cél és koncepció
- Egy áttekinthető mini-katalógus, ahol a felhasználó gyorsan szűr, kártyákból megnyitja a terméket, majd kosárba tesz és összegzést lát, tényleges fizetés nélkül, UI/UX gyakorláshoz ideális.
- A megvalósításhoz választható modern sablon-alapú környezet (pl. WordPress + WooCommerce téma, no-code builder vagy SaaS shop-sablon), így a struktúra gyorsan összerakható és testreszabható.

### Oldalstruktúra
- Főmenü: Kezdőlap, Termékek, Rólunk, Kapcsolat; a Termékek az alapértelmezett fókusz-oldal, hogy a felhasználó azonnal a kínálatba érkezzen.
- Lábléc: rövid bemutatkozás, elérhetőség, hírlevél feliratkozó mező, alap jogi linkek (ÁSZF, adatkezelés) vázlata a későbbi bővítéshez.

### Katalógus oldal (6–9 kártya)
- Rácselrendezés: 3 oszlop desktopon, 2 tablet, 1 mobil; minden kártyán nagy kép, terméknév, ár, egy rövid benefit (max. 6–8 szó), és “Gyors megtekintés” + “Kosárba” gomb.
- Szűrők és rendezés: kategória (pl. Új, Népszerű, Akció), ár csúszka, címkék (anyag/szín), rendezés népszerűség/ár/újdonság szerint; azonnali vizuális visszajelzés a találatszámról.

### Kosár-szimuláció (fizetés nélkül)
- Oldalsó off-canvas kosár: ha a felhasználó “Kosárba” kattint, a kosár panel megnyílik, mutat képet, nevet, árat, darabszám-váltót, részösszeget és egy “Pénztár szimuláció” gombot.
- Pénztár-szimuláció oldal: űrlapmezők mock-kal (név, e-mail, szállítási mód választó), “Rendelés áttekintése” doboz; végül “Szimulált megrendelés beküldése” gomb, ami köszönő képernyőre visz (nincs tényleges fizetés).

### Termékoldal sablon
- Hajtás felett: nagy galéria (1 fő kép + 3–4 bélyeg), terméknév, rövid leírás, kulcs benefit lista 3 pontban, ár, mennyiség választó, “Kosárba” gomb, készlet státusz.
- Hajtás alatt: részletes leírás, specifikációk táblázatban, vásárlói visszajelzés szekció (mock), és “Kapcsolódó termékek” 4 kártyás rácsban a kategória/címkék alapján.

### UI minták és komponensek
- Gombok: primer (CTA) élénk szín, szekunder körvonalas; konzisztens állapotok (hover/active/focus) a tanulhatóságért.
- Kártyák: kerekített sarkok, ár mellett kis “Akció” vagy “Új” címke; egységes ármegjelenítés és tizedes kezelés.

### Tartalmazandó funkciók
- Gyors megtekintés: modálban kép, 1–2 mondatos leírás, ár, “Kosárba” gomb; cél a böngészési súrlódás csökkentése és a kártya → kosár útvonal rövidítése.
- Üres állapotok: ha nincs találat a szűrőre, megjelenik javaslat (szűrők törlése) és 4 ajánlott termék; mindez UX szempontból fontos jelzéssel.

### Példa tartalomváz
- Kategóriák: “Alap darabok”, “Limitált”, “Ajándék” – mindegyikben 2–3 termék, így kijön a 6–9-es katalógus.
- Benefit-példák: “Tartós anyag”, “Gyors szállítás”, “Kézzel készített” – rövidek, mérhető előnyt sugallnak, nem csak jellemzőt.

### Stílusirány
- Betűtípus-páros: egy groteszk család két vastagsággal a sebesség és konzisztencia érdekében; nagy címek, kényelmes sortáv a leírásoknál.
- Színpaletta: 1 primer (CTA), 1 neutrális háttér, 1 sötét szövegszín; sablonban könnyen cserélhető, márkára szabható.

### Gyors megvalósítási út
- Válassz sablon-alapot, ami támogatja katalógus és termékoldal elrendezést, valamint könnyű kosár-kezelést (pl. WooCommerce-kompatibilis téma vagy kész webshop-sablon).
- Tölts fel 6–9 terméket egységes képmérettel (pl. 4:5), írd meg a 3 pontos benefit listát sablonként, majd kapcsold be a szűrő/rendező modulokat és a kosár-panelt.

### Tesztelési ellenőrzőlista
- Mobilon 1 oszlopos rács, fix, jól látható “Kosár” ikon jelzett mennyiséggel; a kosár-panel könnyen bezárható és görgethető.
- Szűrők kombinációja nem okoz “csapda” állapotot; találatszám azonnal frissül; minden gomb fókusz-állapota elérhető billentyűzettel is.

### Bővítési ötletek
- Kívánságlista és “összehasonlítás” modul a döntéstámogatáshoz; később valós fizetési folyamatra is bővíthető ugyanarra az IA-ra.
- Több sablonváltozat: minimal, magazinos kezdőlap, vagy promó blokk a katalógus előtt, szezonális ajánlattal és gyors linkekkel.
