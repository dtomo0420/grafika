# BLENDERBEN MEGVALÓSÍTOTT ELEMEK
## Jelzőlámpa - DeakTamas_CV8RM0.blend
- A jelzőlámpa állványának létrehozása, méretre formázása.
- A jelzőlámpa táblájának létrehozása, méretezése. Az oszlopra valósághű elhelyezése.
- Kereszt létrehozása téglatest megformazásával. Y tengelyre 45/-45 fokkal elforgatás.
- Jelzőtábla további szerkesztése
  - falvastagság beállítása
  - középső rész mozgatása befelé
  - a belső sarkok és a szélső sarkok közötti köztes sarkok mozgatása befelé

## Sorompó állványa - DeakTamas_CV8RM0_2.blend
- Az állványok létrehozása téglatestből, majd ezek pozícionálása.
- A téglatestek felosztása loop cut alkalmazásával.
- A számunkra felesleges oldalakat kijelöljük, majd eltávolítjuk.
- Viszont új oldalakat kell kell behúznunk, kijelöljük az éleket és az F lenyomásával hozzáadjuk az új oldalakat

# THREEJS-BEN MEGVALÓSÍTOTT ELEMEK

## Fények - lights(am, plc, plv)
- három paraméterrel rendelkezik
  - am: ambiens fény erőssége
  - plc: pontfény színe
  - plv: pontfény erőssége
- az alapértelmezett értékük adott, később a nappal/éjszaka gombokkal váltható ezek értéke
- itt ambiens/pontfényt adunk hozzá csak a színtérhez, a reflektorfény más módon kerül hozzáadásra

## Talaj - groundfv()
- síklap (PlaneGeometry) alkotja
- az x tengelyre elforgattam
- egyszerű zöld színt kapott

## Sorompó kiegészítése kereszttel - crossfv()
- 2 db 45, illetve 2 db 135 fokkal elforgatott téglalap alkotja
- az elemek piros színt kaptak

## Sorompó kiegészítése lámpákkal - lampfv()
- 4 db henger alkotja (CylinderGeometry)
- az elemek piros színt kaptak

## Sorompó - gatefv()
- egy henger alkotja (CylinderGeometry)
- metalTexture textúra lett hozzárendelve
- esemény: a képernyőre kattintáskor a sorompó lecsukódik/felnyílik

## Épület - buildingfv()
- az alapzat és a tető 1-1 téglatestből áll (BoxGeometry)
- a kettő testet 1-1 henger köti össze, melyek a már korábban is használt metalTexture-t veszik fel

## Vágányok - tracksfv()
- sínpár
  - a sínek egy-egy téglatestből állnak (BoxGeometry)
  - metalTexture textúra lett hozzárendelve
- keresztalj
  - a vágányok között elhelyezett léc -másnéven keresztalj- egy téglatestből áll (BoxGeometry)
  - treeTexture textúra lett hozzárendelve
  - összesen 80 vágány került elhelyezésre

## Lámpák - lamp()
- a lámpa állvány, illetve felső részét is téglatestek alkotják
- a textúra: treeTexture

## Vagon - wagon()
- alapzat: egy téglatest alkotja (BoxGeometry)
- oldalfalak: szintén téglatestek, megfelelően pozicionálva
- textúra: treeTexture a vagon minden elemére

## Erdő - treefv()
- 70 fa alkotja az erdőt
- 1 fa generálása
  - 1-1 random érték generálása a [-90,90] intervallumon (a,b értékek)
  - 1 random érték generálása a [1,3] intervallumon (b érték)
  - b ha értéke kisebb, mint -15, vagy nagyobb mint 15, akkor helyezzük el a fát, más esetben újat generálunk
  a fa felépítése
  - egy téglatest (BoxGeometry) alkotja a törzsét
  - a törzs treeTexture textúrát kapott
  - a lombkoronát egy gömb (SphereGeometry) alkotja
  - a lomb autumnTexture textúrát kapott






