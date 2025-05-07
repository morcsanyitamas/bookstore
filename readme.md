# Könyvesbolt Projekt

## Történet
Egy könyvesbolt digitális katalógusának fejlesztésén dolgozol. A cél, hogy a könyvek adatait (cím, szerző, kiadás éve, ár) egy Git verziókövető rendszerben tárold, és a csapatod segítségével folyamatosan bővítsd és frissítsd az adatokat. A projekt során meg kell tanulnod a Git alapvető parancsait, a verziókezelés működését, és a csapatmunkához szükséges eszközöket, mint például a konfliktusok kezelése és a változások visszakövetése.

## Feladatok

### Hozz létre egy új lokális repository-t
Hozz létre egy új Git repository-t, és készíts benne egy `books.json` nevű fájlt.

**Feladatok**:
- Hozz létre egy új mappát `bookstore` néven.
- Hozz létre egy új Git repository-t.
- Hozz létre egy `books.json` fájlt, és adj hozzá három könyvet az alábbi adatokkal:
```json
[  
  {
    "cím": "A kőszívű ember fiai",
    "szerző": "Jókai Mór",
    "kiadás_éve": 1869,
    "ár": 3500
  },
  {
    "cím": "Egri csillagok",
    "szerző": "Gárdonyi Géza",
    "kiadás_éve": 1901,
    "ár": 4000
  },
  {
    "cím": "Pál utcai fiúk",
    "szerző": "Molnár Ferenc",
    "kiadás_éve": 1906,
    "ár": 3000
  }
]
```
**Kritériumok**:
- A `books.json` fájl tartalmazza a fenti három könyvet.
- A változtatások legyenek elmentve egy commitban, amelynek üzenete: "Könyvek listájának létrehozása".

### Adj hozzá új könyveket
Bővítsd a könyvek listáját további két könyvvel.

**Feladatok**:
- Adj hozzá két új könyvet a `books.json` fájlhoz:
```bash
{
    "cím": "Az arany ember",
    "szerző": "Jókai Mór",
    "kiadás_éve": 1872,
    "ár": 4500
  },
  {
    "cím": "Tüskevár",
    "szerző": "Fekete István",
    "kiadás_éve": 1957,
    "ár": 3200
  }
```
- Mentsd el a változtatásokat egy új commitban.

**Kritériumok**:
- A `books.json` fájl tartalmazza az új könyveket.
- A commit üzenete legyen: "Új könyvek hozzáadása a listához".

### Hozd létre a remote repository-t
Hozd létre a GitHub-on a `bookstore` repository-t, és töltsd fel ide a lokális repository-t.
**Feladatok**:
- Hozz létre egy új repository-t a GitHub-on `bookstore` néven.
- A repository legyen publikus.
- Állítsd be a lokális repository-t, hogy a GitHub repository-ra mutasson.
- Töltsd fel a lokális repository-t a GitHub-ra.

### Javíts ki egy elírást
A "kiadás_éve" jellemzőt írd át "kiadás-éve"-re.

**Feladatok**:
- Javítsd ki a "kiadás_éve" jellemzőt "kiadás-éve"-re a `books.json` fájlban.
- Mentsd el a változtatásokat egy új commitban, úgy hogy ezt a **GitHub felületén csinálod meg**.

**Kritériumok**:
- A `books.json` fájlban a "kiadás_éve" jellemző helyesen szerepeljen "kiadás-éve"-re.
- A commit üzenete legyen: "Elírás javítása: kiadás_éve -> kiadás-éve".

### Adj hozzá új könyveket
Bővítsd a könyvek listáját az alábbi 5 könyvvel.

**Feladatok**:
- Adj hozzá két új könyvet a `books.json` fájlhoz:
```bash
{
  "cím": "Légy jó mindhalálig",
  "szerző": "Móricz Zsigmond",
  "kiadás-éve": 1920,
  "ár": 2800
},
{
  "cím": "Abigél",
  "szerző": "Szabó Magda",
  "kiadás-éve": 1970,
  "ár": 3700
},
{
  "cím": "A Pál utcai fiúk",
  "szerző": "Molnár Ferenc",
  "kiadás-éve": 1906,
  "ár": 3000
},
{
  "cím": "Kincskereső kisködmön",
  "szerző": "Móra Ferenc",
  "kiadás-éve": 1018,
  "ár": 2500
},
{
  "cím": "Iskola a határon",
  "szerző": "Ottlik Géza",
  "kiadás-éve": 1959,
  "ár": 3600
}
```
- Mivel rájöttél, hogy jobb, ha a kommitokat kisebb egységekben készíted, ezért minden könyvet külön commitban ments el.

**Kritériumok**:
- A `books.json` fájl tartalmazza az új könyveket.
- Minden könyv hozzáadása külön commitban legyen elmentve.
- A commit üzenete legyen: "Új könyv hozzáadása: [könyv címe]".

### Tedd elérhetővé a könyveket a GitHub-on
Töltsd fel a lokális repository-t a GitHub-ra, hogy a csapat többi tagja is hozzáférjen a könyvekhez.

**Feladatok**:
- Töltsd fel a lokális repository-t a GitHub-ra.
- Amennyiben szükséges, oldd fel a konfliktusokat.

### Javíts egy hibát a könyvek listájában
Észrevetted, hogy az egyik könyv árát rosszul adtad meg. Javítsd ki a hibát.

**Feladatok**:
- Javítsd ki "A kőszívű ember fiai" árát 3500 Ft-ról 3700 Ft-ra.
- Mentsd el a változtatást egy új commitban.
- A változtatásokat töltsd fel a GitHub-ra.

**Kritériumok**:
- A `books.json` fájlban a javított ár szerepeljen.
- A commit üzenete megfelelő legyen.

### Javítsd ki a hibát
Javítsd ki a "Kincskereső kisködmön" című könyv kiadás évét 1918-ra.

**Feladatok**:
- Javítsd ki a "Kincskereső kisködmön" című könyv kiadás évét 1918-ra.
- Mentsd el a változtatást egy új commitban.
- A változtatásokat töltsd fel a GitHub-ra.

**Kritériumok**:
- A `books.json` fájlban a javított kiadás év szerepeljen.
- A commit üzenete megfelelő legyen.

### Kedvezmény bevezetése
Hozz létre egy branchet `feature/add-discounts` néven, és adj hozzá egy új tulajdonságot a könyvek listájához, amely a tartalmazza a kedvezmény mértékét.

**Feladatok**:
- Hozz létre egy új branch-et.
- Adj hozzá egy "Kedvezmény" tulajdonságot a `books.json` fájlhoz.
- A változtatásokat töltsd fel a GitHub-ra, a megfelelő branche-re.

**Kritériumok**:
- Az új branch neve legyen `feature/add-discounts`.
- A `books.json` fájl tartalmazza a kedvezményeket.
- A kedvezmény egy %-os érték legyen, véletlenszerűen válaszd ki az értékeket 5% és 25% között.
- Legyen legalább egy commit a branchen.

### Raktárkészlet bevezetése
Hozz létre egy új branchet `feature/add-stock` néven, és adj hozzá egy új tulajdonságot a könyvek listájához, amely tartalmazza a könyvek raktárkészletét.

**Feladatok**:
- Hozz létre egy új branch-et `feature/add-stock` néven.
- Adj hozzá egy "Raktárkészlet" tulajdonságot a `books.json` fájlhoz, amely minden könyvnél egy számot tartalmaz (pl. 10, 20, 30).
- A változtatásokat töltsd fel a GitHub-ra, a megfelelő branche-re.

**Kritériumok**:
- Az új branch neve legyen `feature/add-stock`.
- A `books.json` fájl tartalmazza a "Raktárkészlet" tulajdonságot minden könyvnél.
- A raktárkészlet értékei legyenek véletlenszerűen kiválasztva 5 és 50 közötti értékekből.
- Legyen legalább egy commit a branchen.

### Kedevezmény bevezetése a main bracnchre
Merge-eld a `feature/add-discounts` branchet a `main` branchre. 

**Feladatok**:
- Merge-eld a branchet.
- Amnennyiben felmerül, old fel a konfliktust úgy, hogy a `books.json` fájl tartalma helyes legyen.
- Merge után töltsd fel a változtatásokat a GitHub-ra.

**Kritériumok**:
- A `main` branch tartalmazza a "kedvezmény" adatokat.

### Raktárkészlet bevezetése a main branchre
Merge-eld a `feature/add-stock` branchet a `main` branchre.

**Feladatok**:
- Merge-eld a branchet.
- Amennyiben felmerül, old fel a konfliktust úgy, hogy a `books.json` fájl tartalma helyes legyen.
- Merge után töltsd fel a változtatásokat a GitHub-ra.

**Kritériumok**:
- A `main` branch tartalmazza a "raktárkészlet" adatokat.

### Jelöljd meg az első 10 könyv felvitelét
Jelöld meg a main branch állapotát egy címkével, ahol az első 10 könyv ára immár helyesen szerepel, valamint a könyvekre vonatkozó kedvezmények és raktárkészlet jellemzők is megjelentek.

**Feldatok**:
- Hozz létre egy címkét `v1.0` néven.
**Kritériumok**:
- A címke neve legyen `v1.0`.
- A címke a `main` branch megfelelő commitjára mutasson.

### Új jellemző hozzáadása: Nyelv
Hozz létre egy új branchet `feature/add-language` néven, és adj hozzá egy új tulajdonságot a könyvek listájához, amely tartalmazza a könyvek nyelvét.

**Feladatok**:
- Hozz létre egy új branch-et `feature/add-language` néven.
- Adj hozzá egy "Nyelv" tulajdonságot a `books.json` fájlhoz, amely minden könyvnél egy szöveges értéket tartalmaz (pl. "magyar", "angol").
- Hozz létre egy pull requestet a `feature/add-language` branchre, és merge-eld a `main` branchre.

**Kritériumok**:
- Az új branch neve legyen `feature/add-language`.
- A `books.json` fájl tartalmazza a "Nyelv" tulajdonságot minden könyvnél.
- A nyelv értékei legyenek a könyvek eredeti nyelvei (pl. magyar könyvek esetén "magyar").
- Legyen legalább egy commit a branchen.

### Korrekció bevezetése
A "Pál utcai fiúk" könyv tévesen, - többször - szerepel a `books.json` fájlban. A második előfordulása helyére vidd fel a következő könyvet:
```json
{
  "cím": "A funtineli boszorkány",
  "szerző": "Wass Albert",
  "kiadás-éve": 1943,
  "ár": 4200,
  "kedvezmény": 10,
  "raktárkészlet": 20,
}
```

### `.gitignore` fájl létrehozása
Hozz létre egy `.gitignore` fájlt, amely kizárja a `*.tmp` kiterjesztésű fájlokat a verziókövetésből.
**Feladatok**:
- Hozz létre egy `.gitignore` nevű fájlt a repository gyökérkönyvtárában.
- Hozz létre egy `test.tmp` nevű fájlt a repository-ban, és ellenőrizd, hogy a Git figyelmen kívül hagyja azt.
**Kritériumok**:
- A `.gitignore` fájl tartalmazza a megfelelő szabályt.
- A `test.tmp` fájl ne jelenjen meg a `git status` kimenetében.
- A `.gitignore` fájl legyen elmentve egy commitban.

### Új könyv hozzáadása
Adj hozzá egy új könyvet a `books.json` fájlhoz az alábbi adatokkal.
**Feladatok**:
- Adj hozzá egy új könyvet a `books.json` fájlhoz:
  ```json
  {
    "cím": "A láthatatlan ember",
    "szerző": "Gárdonyi Géza",
    "kiadás-éve": 1902,
    "ár": 3900
  }
  ```
- A változtas bevezetése után jutott eszedbe, hogy ezt egy új branch-en szeretnéd elvégezni, ezért hozz létre egy új branchet `feature/add-invisible-man` néven.
- Az eddigi változtatásokat mentsd el egy stashban, hozd létre az új branch-et, és alkalmazd a stashben lévő változtatásokat.
- Mentsd el a változtatásokat egy commitban.

### A "láthatatlan ember" bevezetése a main branchre
A Cherry-pick parancs segítségével vidd át a `feature/add-invisible-man` branchen lévő commitot a `main` branchre.
**Feladatok**:
- Használj cherry-pick parancsot a `feature/add-invisible-man` branchen lévő commit átvitelére a `main` branchre.
- Amennyiben felmerül, oldd fel a konfliktust úgy, hogy a `books.json` fájl tartalma helyes legyen.
**Kritériumok**:
- A `main` ág tartalmazza a "láthatatlan ember" könyvet.

### Nagybetűsítés
A könyvek jellemzőit nagybetűsítve szeretnéd látni a books.json fájlban
**Feladatok**:
- Hozz létre egy új branch-et `feature/capitalize-attributes` néven.
- Használj egy scriptet, amely nagybetűsítve írja ki a könyvek jellemzőit a `books.json` fájlban.
- Mentsd el a változtatásokat egy commitban.
**Kritériumok**:
- Az új branch neve legyen `feature/capitalize-attributes`.
- A `books.json` fájl tartalmazza a nagybetűsített jellemzőket.
- Legyen legalább egy commit a branchen.

### Oldalszám hozzáadása
Vezesd be a könyvekhez tartalmazó oldalszámot a `books.json` fájlban.
**Feladatok**:
- Hozz létre egy új branch-et `feature/add-page-count` néven.
- Adj hozzá egy "Oldalszám" tulajdonságot a `books.json` fájlhoz, amely minden könyvnél egy számot tartalmaz (pl. 200, 300).
- Mentsd el a változtatásokat egy commitban.
**Kritériumok**:
- Az új branch neve legyen `feature/add-page-count`.
- A `books.json` fájl tartalmazza az "Oldalszám" tulajdonságot minden könyvnél.
- Az oldalszám értékei legyenek véletlenszerűen kiválasztva 100 és 1000 között.
- Legyen legalább egy commit a branchen.

### Mergeld a `feature/capitalize-attributes` branchet a `main` branchre
**Feladat**: Merge-eld a `feature/capitalize-attributes` branchet a `main` branchre.
**Kritériumok**:
- A `main` ág tartalmazza a nagybetűsített jellemzőket.
- A merge során oldd fel a konfliktusokat, ha szükséges.

### Aktualizáld a `feature/add-page-count` branchet a `main` branch alapján
**Feladat**: Frissítsd a `feature/add-page-count` branchet a `main` branch alapján.
**Kritériumok**:
- A `feature/add-page-count` branch tartalmazza a `main` branch legfrissebb változásait, vagyis a nagybetűsített jellemzőket.
- A main branch változtatásai legyenek rebase-elve a `feature/add-page-count` branchre.
- A konfliktusok legyenek feloldva, és a `books.json` fájl tartalma helyes legyen.
