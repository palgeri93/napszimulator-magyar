# Nap-szimulátor magyarul

Az évszakok és a Nap látszólagos égi útjának interaktív szimulátora,
az eredeti megjelenést megtartó magyar feliratokkal.

## Használat

A GitHub Pages oldalon közvetlenül használható, telepítés nélkül.
A dátumot az alsó csúszka, a földrajzi szélességet a piros kör vagy a
megfigyelő alakjának húzásával lehet állítani. A bal oldali térbeli ábra
forgatható. Az „indítás” gomb elindítja az év folyamatos szimulációját.

## Technológia

Az oldal statikus HTML és helyben tárolt Ruffle 0.7.1 JavaScript/WebAssembly
futtatókörnyezet. A lefordított SWF az eredeti szimuláció működését őrzi meg;
ez nem a szimuláció teljes JavaScript-átírása. A fájlhivatkozások relatívak,
így a GitHub Pages projekt alatti útvonalon is működnek.

Helyi kipróbálás: `python -m http.server 8000`, majd
`http://localhost:8000/` megnyitása.

## Közzététel

A mellékelt GitHub Actions munkafolyamat a `main` ágra küldött változásokból
publikál. A tároló Settings → Pages részében a forrás legyen GitHub Actions.

## Forrásmegjelölés

- Eredeti szimulátor: [Nebraska Astronomy Applet Project](https://astro.unl.edu/).
- Eredeti verzió: eclipticSimulator024, 2009. március 19.
- Ez magyar adaptáció, nem az eredeti alkotók hivatalos kiadása.
- Az eredeti szimulátor szerzői jogai az eredeti jogosultaknál maradnak.
- Az eredeti fájl engedélyszövege nem kereskedelmi, változatlan felhasználást
  említ; a magyar adaptációra nem állítunk önálló nyílt forrású licencet.
- [Ruffle](https://ruffle.rs/): MIT / Apache-2.0; a licencek a `ruffle` mappában.
