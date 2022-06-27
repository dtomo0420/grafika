# Számítógépes grafika gyakorlat beadandó feladat
A feladat egy vasúti terepasztal modellezése Three.js-ben az alábbiak szerint.
A beadott csomag mérete maximum 8 MB lehet a Coospace beállítása miatt.

## Fő elemek
- A színtér – Talaj, vasútállomás, stilizált vonat, hegyek, stb.
- A színtér legyen teljes mértékben megnézhető. Szükség esetén billentyűk/egér segítségével az épületek falai legyenek eltüntethetők.
- Egy komplex épület/jármű előállítása. Lehet stilizált is, de ha beépített Three.js geometriákból van, akkor legalább 5-5 elemből kell állniuk.
- Legalább 3 különböző alak/tárgy (pl. ember, vonat, egyéb jármű, stb.).

## Minimálisan szükséges, statikus geometriai modellek (2+2 pont)
- Beépített Three.js geometriák használata (2 pont).
- Blender geometriai modellezés (2 pont).
    - A fenti geometriák közül legalább 2 legyen Blender-ben lemodellezett.
    - A beépített Blender hálók legyenek jól látható módon továbbszerkesztve!
    - A modelleket .blend formátumban is mentse el és csatolja beküldéskor!
    - Külön szöveges fájlban adjon rövid leírást a felszínhálók elkészítésének fontosabb lépéseiről! Miből indult ki, milyen szerkesztések történtek, stb.
    
Amennyiben a teljes, vagy majdnem a teljes színteret Blender-ben valósítja meg a hallgató, és ezt betöltve jeleníti meg Three.js-ben, akkor a beadandó feladat nem lesz kiértékelve, és automatikusan 0 pontot adunk rá!

## Animáció (3 pont)
- Legalább 2 animált tereptárgy.
  - Legalább 1 db animáció, amely billentyűk vagy egér segítségével mozgatható.
  - Legalább 1 db animáció, amely időzítő segítségével önállóan mozog.
- Animáció példák: fénysorompó fényei villognak, vonat mozog, emberek „sétálnak”, elszabadult bőrönd gurul a rámpán, stb.

## Interakció (2 pont)
- A színteret körbe lehessen forgatni egérrel és/vagy a kurzormozgató billentyűk segítségével.
- A megvilágítás interaktív beállításával nappal és éjszaka választható legyen.
- Az ablak bal felső sarkában jelenjen meg a programot készítő hallgató neve, NEPTUN azonosítója, valamint a szakja és az aktuális tanév megnevezése.
- Az ablak jobb felső sarkában jelenjen meg a használható billentyűk felsorolása a funkciók megadásával együtt.
- A szöveges információkat ki/be lehessen kapcsolni az „I” (mint Ilona) billentyűvel.
 
## Megvilágítás (2 pont)
- Ambiens fény.
- Legalább 2 db be-kikapcsolható pontfény vagy reflektorfény (lámpa, reflektor, fénysorompó, nap, hold, …).
- Nappal és éjszaka váltás lehetősége.
- Megvilágításra alkalmas anyag objektum (Lambert vagy Phong).

## Textúra (1 pont)
- Legalább 2 db objektum egymástól független, értelmes textúrázása (talaj, vonat, stb.).