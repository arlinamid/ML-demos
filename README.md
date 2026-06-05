# Forge Lab

Interaktiv gepi tanulas demok magyar magyarazatokkal.

A projekt ket fo iranyt mutat be:

- **Neural Forge**: keziras-, szam- es betufelismeres eloben tanithato MLP haloval.
- **Optic Forge**: kepfelismeres MobileNet/ImageNet alapon, feature-map es figyelem-hoterkep nezettel.

## Inditas

Nyisd meg az `index.html` fajlt bongeszoben.

Innen elerheto:

- `neural-forge-learn-v2.html` - Neural Forge V2, 0-9 + A-Z felismeressel
- `neural-forge-learn.html` - eredeti szamos Neural Forge demo
- `optic-forge-v3-full.html` - Optic Forge V3 teljes ImageNet/WordNet metaadattal
- `optic-forge.html` - Optic Forge alap verzio

## Fajlok

| Fajl | Leiras |
| --- | --- |
| `index.html` | Landing oldal a Neural Forge es Optic Forge demokhoz. |
| `neural-forge-learn-v2.html` | Szam- es nagybetufelismero MLP demo, sajat rajzzal tanithato. |
| `neural-forge-learn.html` | Eredeti szamfelismero tanulo demo. |
| `optic-forge-v3-full.html` | Kepfelismero demo ImageNet/WordNet metaadatokkal, hoterkeppel. |
| `optic-forge-v2.html` | Korabbi Optic Forge valtozat. |
| `optic-forge.html` | Optic Forge alapvaltozat. |

## Neural Forge V2

A Neural Forge V2 egy tiszta JavaScriptben futtathato MLP halot mutat be:

- bemenet: `14x14 = 196` pixel
- rejtett retegek: `48` es `32` neuron
- kimenet: `36` osztaly, `0-9` es `A-Z`

A demo rajzvasznat, elofeldolgozott 14x14-es kepet, softmax kimenetet, tanitasi grafikat es 3D halovizualizaciot mutat. A sajat rajzok hozzaadhatok a tanitohalmazhoz.

## Optic Forge

Az Optic Forge kepfelismeresi demo:

- top-5 ImageNet osztalyokat jelenit meg
- WordNet/ImageNet metaadatot hasznal a jobb ertelmezeshez
- feature-map-eket rajzol
- occlusion-alapu figyelem-hoterkepet keszit

Kamera vagy feltoltott kep is hasznalhato, ha a bongeszo es a kornyezet engedi.

## Technikai megjegyzesek

- A demok standalone HTML fajlok.
- A Three.js, TensorFlow.js es egyes konyvtarak CDN-rol toltodnek be, ezert internetkapcsolat kellhet.
- Helyi fajlkent is megnyithatok, de egyes bongeszok a kamera- vagy halozati funkciokat korlatozhatjak.
- A Neural Forge V2 szintetikus tanitoadatot general bongeszoben, kulso adatletoltes nelkul.

## Cel

A cel nem rekordpontossagu modell epites, hanem a gepi tanulas lathatova tetele: mit kap bemenetkent a halo, hogyan alakul a belso allapot, hogyan jon ki a tipp, es mit jelent a tanitas vagy a figyelem egy vizualis peldan.
