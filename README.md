# Humanizer Magyar

Claude Code / Claude.ai skill, ami AI-generált **magyar** szövegekből tünteti el a jellegzetes AI-jeleket. Magyar nyelvi sajátosságokra hangolva — nem egyszerű fordítása az angol verziónak.

A [`blader/humanizer`](https://github.com/blader/humanizer) ihlette, de a hangsúlyt a magyar nyelvre jellemző AI-mintákra helyezi: bürokratikus passzív (*“kerül megrendezésre”*), igekötős túlhasználat, magyar AI-szókincs (*elengedhetetlen, kulcsfontosságú, exponenciálisan*), birtokos láncok, anglicizmusok és tipográfiai hibák.

## Miért külön magyar verzió?

Amikor angol humanizer-szabályokat alkalmaztam magyar szövegre, a legárulkodóbb AI-jelek **átsiklottak** a hálón:

- A magyar AI-szöveg csúcstüneménye, a `kerül + igenév` szerkezet (*“a konferencia megrendezésre kerül”*) angolban nem létezik.
- Az AI-favorit magyar szavak (*elengedhetetlen, kulcsfontosságú, kiemelkedő*) más szótár, mint az angol megfelelőik.
- A magyar idézőjel-szabály (`„..."`) különbözik az angoltól.
- A magyar címekben sentence case van, nem Title Case.
- A “végső soron”, “a nap végén” típusú anglicizmusok specifikus calque-ok.

A skill 30 mintát kategorizál öt csoportban: tartalom, szókincs, nyelvtan, tipográfia, diskurzus.

## Mit tartalmaz

```
humanizer-magyar/
├── SKILL.md             # Fő skill-fájl — 30 minta példákkal
├── manifest.json        # Csomag-metaadat
├── README.md            # Ez a fájl
├── LICENSE              # MIT
└── references/
    ├── szokincs.md      # Bővített AI-szókincs táblázatok
    ├── tipografia.md    # Magyar tipográfiai szabályok (idézőjel, kötőjel, számformázás)
    └── peldak.md        # 10 átírási példa (energia, IT, email, akadémiai, marketing, LinkedIn, vezetői üzenet, szerződés)
```

## Telepítés

### Claude.ai (web vagy desktop)

1. Töltsd fel a `humanizer-magyar.skill` ZIP-fájlt a Claude beállításai között a “Skills” szekcióban.
1. Ha kézzel akarod, csomagold ki, és töltsd fel a `SKILL.md`-t a referencia-fájlokkal együtt.

### Claude Code

```bash
mkdir -p ~/.claude/skills/humanizer-magyar
unzip humanizer-magyar.skill -d ~/.claude/skills/
```

Vagy git-tel közvetlenül:

```bash
git clone <repo-url> ~/.claude/skills/humanizer-magyar
```

### OpenCode

```bash
mkdir -p ~/.config/opencode/skills/humanizer-magyar
unzip humanizer-magyar.skill -d ~/.config/opencode/skills/
```

## Használat

### Trigger-mondatok (magyar)

A skill automatikusan aktiválódik, ha a kérésedben szerepel:

- *“humanizáld ezt a szöveget”*
- *“tedd emberibbé”* / *“természetesebbé”*
- *“vedd ki belőle az AI-jeleket”*
- *“AI-tüskék kiszedése”*
- *“magyarosítsd”* (stilisztikai értelemben)

### Trigger-parancs (Claude Code / OpenCode)

```
/humanizer-magyar

[ide jön a humanizálandó szöveg]
```

### Példa-promptok

```
Humanizáld ezt a magyar szöveget:
[szöveg]
```

```
Vedd ki ebből a magyar szövegből az AI-jeleket. Ne csak szót cserélj, írd át,
ahol kell:
[szöveg]
```

```
Stilisztikai szerkesztés: a beszámoló közvetlenebb hangú legyen.
[szöveg]
```

### Hangkalibrálás (saját stílus átvétele)

Ha azt szeretnéd, hogy a humanizált változat a te írásodra hasonlítson, mellékelj egy mintát:

```
Itt egy minta a saját írásomból, ezt a stílust kövesd:
[2-3 bekezdés a saját írásodból]

Most humanizáld ezt:
[az AI-szöveg]
```

A skill elemzi a mondathosszt, szókincs-szintet, központozási szokást és visszatérő fordulatokat, majd ezekhez igazítja az átírást.

## Mire figyel külön a magyar verzió

|Kategória             |Példa-minta                                                                              |
|----------------------|-----------------------------------------------------------------------------------------|
|Tartalom              |Túlhajtott jelentőség (*mérföldkő, korszakalkotó*), homályos forrás (*szakértők szerint*)|
|Szókincs              |*Elengedhetetlen, kulcsfontosságú, kiemelkedő, exponenciálisan, holisztikus, robusztus*  |
|Idegen szavak         |*Implementál, optimalizál, fókuszál* (ahol van magyar megfelelő)                         |
|Bürokratikus passzív  |*Kerül megrendezésre → megrendezzük* — a legtipikusabb magyar AI-jel                     |
|Igekötős túlhasználat |*Kihangsúlyoz, megalapoz, kibontakozik*                                                  |
|Nominalizáció         |*-ás/-és* halmozás ige helyett                                                           |
|Birtokos láncok       |*A vállalat digitalizációjának folyamatának eredménye*                                   |
|*Amely*-mellékmondatok|Halmozott vonatkozói szerkezetek                                                         |
|Tipográfia            |Idézőjel (`„..."` nem `"..."`), Title Case, gondolatjel-mánia                            |
|Diskurzus             |*Összegzésképpen elmondható…, A jövő ígéretes…, Természetesen!*                          |
|Anglicizmus           |*A nap végén, végső soron*                                                               |

A teljes 30 minta a `SKILL.md`-ben.

## Példa

**Előtte (AI-magyar):**

> A digitalizációs stratégia új fejezetet nyit a vállalat életében, mérföldkő az iparág digitális átalakulásának folyamatában, és kiemelt szerepet tölt be a hosszú távú versenyképesség biztosításában.

**Utána:**

> A vállalat 2025 januárjától felhőalapú adatkezelésre vált, és három évre 12 milliárd forintot különít el a háttérrendszerek cseréjére.

## Workflow

A skill háromlépcsős workflow-t követ minden átíráskor:

1. **Első átírás** (Draft) — minták azonosítása és cseréje
1. **Audit** — *“Mitől hangzik még mindig AI-szerűnek?”* — saját kritika
1. **Végső átírás** (Final) — az audit alapján finomítva

Ez a duplapasszos megközelítés a `blader/humanizer`-ből származik — a magyar verzió is megtartja, mert magyar szövegnél is működik.

## Hivatkozások

- [`blader/humanizer`](https://github.com/blader/humanizer) — angol kiindulás, 13.8k csillag
- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) — alapminta-katalógus
- A magyar minták saját megfigyelésen és magyar szövegszerkesztői gyakorlaton alapulnak

## Hozzájárulás

Ha új AI-mintát figyelsz meg magyar szövegekben, vagy egy átírási példa nem működik:

1. Nyiss issue-t / küldj üzenetet előtte/utána szöveggel.
1. Indokold röviden, miért gondolod AI-jelnek (nem stilisztikai preferencia).
1. Adj 2-3 példát ugyanarra a mintára különböző kontextusból.

## Licenc

MIT — szabadon használhatod, módosíthatod, megoszthatod.

## Verzió

1.0.0 — első kiadás, 30 minta, 4 kategorizált fájl.