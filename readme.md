
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
- Állítsd be a lokális repository-t, hogy a GitHub repository-ra mutasson.
- Töltsd fel a lokális repository-t a GitHub-ra.

### Javíts ki egy elírást
A "kiadás_éve" jellemzőt írd át "kiadás-éve"-re.
**Feladatok**:
- Javítsd ki a "kiadás_éve" jellemzőt "kiadás-éve"-re a `books.json` fájlban.
- Mentsd el a változtatásokat egy új commitban, úgy hogy ezt a GitHub felületén csinálod meg.
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
**Kritériumok**:
- A `books.json` fájlban a javított ár szerepeljen.
- A commit üzenete megfelelő legyen.

### Javítsd ki a hibát
Javítsd ki a "Kincskereső kisködmön" című könyv kiadás évét 1918-ra.
**Feladatok**:
- Javítsd ki a "Kincskereső kisködmön" című könyv kiadás évét 1918-ra.
- Mentsd el a változtatást egy új commitban.
**Kritériumok**:
- A `books.json` fájlban a javított kiadás év szerepeljen.
- A commit üzenete megfelelő legyen.

### Kedvezmény bevezetése
Hozz létre egy branchet `feature/add-discounts` néven, és adj hozzá egy új tulajdonságot a könyvek listájához, amely a tartalmazza a kedvezmény mértékét.
**Feladatok**:
- Hozz létre egy új branch-et.
- Adj hozzá egy "Kedvezmény" tulajdonságot a `books.json` fájlhoz.
- Mentsd el a változtatásokat egy commitban.
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
- Mentsd el a változtatásokat egy commitban.

**Kritériumok**:
- Az új branch neve legyen `feature/add-stock`.
- A `books.json` fájl tartalmazza a "Raktárkészlet" tulajdonságot minden könyvnél.
- A raktárkészlet értékei legyenek véletlenszerűen kiválasztva 5 és 50 közötti értékekből.
- Legyen legalább egy commit a branchen.

### Kedevezmény bevezetése a main bracnchre
**Feladat**: Merge-eld a `feature/add-discounts` branchet a `main` branchre. 
**Teendők**:
- Merge-eld az ágat.
- Amnennyiben felmerül, oldd fel a konfliktust úgy, hogy a `books.md` fájl tartalma helyes legyen.
**Kritériumok**:
- A `main` ág tartalmazza a "kedvezmény" adatokat.

### Raktárkészlet bevezetése a main branchre
**Feladat**: Merge-eld a `feature/add-stock` branchet a `main` branchre.
**Teendők**:
- Merge-eld az ágat.
- Amennyiben felmerül, oldd fel a konfliktust úgy, hogy a `books.md` fájl tartalma helyes legyen.
**Kritériumok**:
- A `main` ág tartalmazza a "raktárkészlet" adatokat.

### Jelöljd meg az első 10 könyv felvitelét
Jelöld meg a main ág állapotát egy címkével, ahol az első 10 könyv ára immár helyesen szerepel, valamint a könyvekre vonatkozó kedvezmények és raktárkészlet jellemzők is megjelentek.
**Feldatok**:
- Hozz létre egy címkét `v1.0` néven.
**Kritériumok**:
- A címke neve legyen `v1.0`.
- A címke a `main` ág megfelelő commitjára mutasson.

### Új jellemző hozzáadása: Nyelv
Hozz létre egy új branchet `feature/add-language` néven, és adj hozzá egy új tulajdonságot a könyvek listájához, amely tartalmazza a könyvek nyelvét.
**Feladatok**:
- Hozz létre egy új branch-et `feature/add-language` néven.
- Adj hozzá egy "Nyelv" tulajdonságot a `books.json` fájlhoz, amely minden könyvnél egy szöveges értéket tartalmaz (pl. "magyar", "angol").
- Mentsd el a változtatásokat egy commitban.
**Kritériumok**:
- Az új branch neve legyen `feature/add-language`.
- A `books.json` fájl tartalmazza a "Nyelv" tulajdonságot minden könyvnél.
- A nyelv értékei legyenek a könyvek eredeti nyelvei (pl. magyar könyvek esetén "magyar").
- Legyen legalább egy commit a branchen.
- Hozz létre egy pull requestet a `feature/add-language` branchre, és merge-eld a `main` branchre.

