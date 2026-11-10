# România 2028 – Simulator de reorganizare administrativă

Extinderea la toată țara a simulatorului *Brăila 2028*: cele 3.180 de UAT din România (fără București), cu execuția bugetară 2025 și populația din Recensământul 2021.

## Ce face

- **Propunerea**: pentru un prag minim de populație pe zonă (3.000 – 15.000 de locuitori), arată câte UAT ar rezulta la nivel național și pe fiecare județ, economia estimată și cât din funcționare își acoperă zonele din venituri proprii.
- **Hartă actuală**: situația de azi a fiecărei primării (acoperirea funcționării din venituri proprii), cu toți indicatorii.
- **Construiește zone**: comasări desenate manual, județ cu județ, cu calculul economiilor și ipoteze modificabile.
- **Propunere automată**: variantele calculate pentru fiecare județ și prag.
- **Regiuni**: regionalizarea pe județe întregi – 8 regiuni de dezvoltare, 8 regiuni istorice, 21 de județe mari (fără modificarea Constituției) sau o variantă construită pe hartă. Pentru fiecare: populația, capitala aleasă, acoperirea din venituri proprii și economia la comasarea consiliilor județene, separat și împreună cu comasarea UAT.

## Date

| Fișier | Conținut |
|---|---|
| `uat_2025.json` | 3.181 UAT: SIRUTA, nume, județ, tip, populație RPL 2021, CIF, suprafață, centru, 10 indicatori financiari 2025, vecinătăți |
| `date_transparenta_2025.tsv` | indicatorii financiari pe CIF și SIRUTA, inclusiv consiliile județene și sectoarele Capitalei |
| `scenarii.json` | propunerile automate pe județ și prag |
| `regiuni.json` | bugetele 2025 ale celor 41 de consilii județene, reședințele de județ și variantele de regiuni |
| `ro_uat.topojson` | contururile UAT (id = cod SIRUTA) |

**Surse**: execuția bugetară la 31.12.2025 a bugetului local, ordonator principal, din rapoartele Ministerului Finanțelor, preluate prin [transparenta.eu](https://transparenta.eu). Pentru cele 44 de UAT din Brăila, toți cei 10 indicatori coincid la leu cu rapoartele COFOG3 descărcate direct de la MF. Populația: INS, RPL 2021. Contururi: geo-spatial.org (ANCPI), cu Victoria (BV), Bălan și Băile Tușnad completate din OpenStreetMap.

## Publicare pe GitHub Pages

1. Creează un repository nou (de exemplu `Romania-Reforma`).
2. Încarcă toate fișierele din acest dosar, în rădăcina repository-ului (`index.html`, `README.md` și fișierele de date).
3. Settings → Pages → Branch `main`, folder `/ (root)` → Save.

Aplicația trebuie servită de un server web (GitHub Pages merge); deschisă direct din fișier, browserul blochează încărcarea datelor.
