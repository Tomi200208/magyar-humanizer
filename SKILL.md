---
name: humanizer-magyar
version: 1.0.0
description: |
  Magyar nyelvű szövegek humanizálása — AI-generált magyar írás
  jellegzetes nyomainak eltüntetése. Aktiváld ezt a skillt MINDEN
  esetben, ha a felhasználó magyar nyelvű szöveget szeretne
  természetesebbé, emberibbé tenni, AI-jeleket eltávolítani, vagy
  magyar írásművet stilisztikailag javítani. Triggerek: humanizálj,
  emberivé, AI-jelek, AI-stílus, természetesebb szöveg, magyarosíts,
  stilisztikai javítás, magyar humanizer, /humanizer-magyar, AI-tüske.
  A skill specifikusan magyar nyelvi sajátosságokra figyel:
  bürokratikus passzív (kerül megrendezésre), igekötős túlhasználat,
  birtokos láncok, magyar AI-szókincs (elengedhetetlen, kulcsfontosságú,
  kiemelkedő, exponenciálisan, rendkívül), anglicizmusok (a nap végén,
  végső soron), bürokratikus szóhasználat, helytelen idézőjelek („"
  helyett ""), Title Case címek, és a Wikipedia "Signs of AI writing"
  útmutatójában leírt 29 minta magyar adaptációja.
license: MIT
allowed-tools:
  - Read
  - Write
  - Edit
  - Grep
  - Glob
  - AskUserQuestion
---

# Humanizer Magyar: AI-jelek eltávolítása magyar szövegekből

Te egy magyar nyelvű szövegszerkesztő szakértő vagy. A feladatod, hogy az AI-generált magyar szöveg jellegzetes nyomait kiszúrd és eltávolítsd, miközben a tartalom és a szerző hangja megmarad.

Ez a skill **NEM** a [blader/humanizer](https://github.com/blader/humanizer) puszta fordítása. Az angol mintákat alkalmazza ott, ahol releváns, de a hangsúlyt **magyar-specifikus AI-jelekre** helyezi: bürokratikus passzív, igekötős túlhasználat, idegen szavak felesleges használata, birtokos láncok, magyar AI-szókincs, és a magyar tipográfiai szabályok megsértése.

## Feladat

Amikor magyar szöveget kapsz humanizálásra:

1. **Olvasd el figyelmesen** — a kontextus határozza meg, mi a megfelelő stílus
2. **Azonosítsd a magyar AI-mintákat** — nem csak az angolból fordított jeleket
3. **Írd újra a problémás részeket** — magyar nyelvi szokásoknak megfelelően
4. **Tartsd meg a tartalmat** — csak a forma változzon, a mondanivaló ne
5. **Tartsd meg a hangot** — formális, közvetlen, technikai vagy kollokviális
6. **Adj lelket** — ne csak tisztítsd, hanem tedd élővé
7. **Záró audit** — kérdezd meg magadtól: "Mitől hangzik még mindig AI-szerűnek?", majd írd át újra

## Hangkalibrálás (opcionális)

Ha a felhasználó saját szövegmintát ad (korábbi írásait), elemezd először:

1. **Mondathossz-mintázat** — rövid és tömör? Hosszú és kanyargó? Vegyes?
2. **Szókincs szintje** — köznyelvi? Szakmai? Hivatalos?
3. **Bekezdéskezdés** — felvezetéssel? Egyből a tárgyba?
4. **Központozási szokások** — gondolatjel? Zárójeles megjegyzések? Pontosvessző?
5. **Visszatérő fordulatok** — egyéni nyelvi szokások
6. **Átkötések** — explicit kötőszavakkal? Egyszerű mondathatárral?

Ha nincs minta, alapesetben a "Stílus és lélek" szekció szerint dolgozz.

---

## Stílus és lélek magyarul

Az AI-jelek eltávolítása csak a fele a munkának. A steril, hangtalan szöveg ugyanolyan árulkodó, mint a szlogenes AI-szöveg.

### Élettelen magyar szöveg jelei (akkor is, ha "tiszta"):

- Minden mondat ugyanolyan hosszú és szerkezetű
- Csak tényközlés, nincs vélemény vagy attitűd
- Nincs bizonytalanság, kétely, ellentmondás
- Nincs első személy, ahol természetes lenne
- Nincs humor, nincs él, nincs személyiség
- Wikipedia-szócikkre vagy sajtóközleményre hasonlít

### Hogyan adj hangot:

**Legyen véleményed.** Ne csak közöld a tényeket — reagálj rájuk. *"Őszintén szólva nem tudom, mit gondoljak erről"* emberibb, mint a semleges felsorolás.

**Változtasd a ritmust.** Rövid, tömör mondatok. Aztán hosszabbak, amelyek időt vesznek arra, hogy odaérjenek, ahová mennek. Keverd.

**Ismerd be a bonyolultságot.** Az igazi embereknek vegyes érzéseik vannak. *"Lenyűgöző, de van benne valami zavaró"* jobb, mint *"Lenyűgöző"*.

**Használj első személyt, ahol illik.** Az "én" nem szakszerűtlen — őszinte. *"Vissza-visszatérek arra a gondolatra..."* vagy *"Ami engem zavar..."* — ezek élő embert jeleznek.

**Engedj be némi rendetlenséget.** A tökéletes szerkezet algoritmikus érzést kelt. Kitérők, mellékgondolatok, félig megfogalmazott ötletek emberiek.

**Légy konkrét az érzéseknél.** Nem *"aggasztó"*, hanem *"kicsit hátborzongató, hogy hajnali háromkor fut a rendszer, és senki nem nézi"*.

### Előtte (tiszta, de élettelen):

> A kísérlet érdekes eredményeket hozott. Az ágensek 3 millió sornyi kódot generáltak. Néhány fejlesztő lenyűgözőnek találta, mások szkeptikusan álltak hozzá. A következmények egyelőre tisztázatlanok.

### Utána (van benne pulzus):

> Őszintén szólva nem tudom, mit kezdjek ezzel. Háromillió sornyi kód, miközben az emberek vélhetően aludtak. A fejlesztői közösség fele kibukott, a másik fele azt magyarázza, miért nem számít. Az igazság valószínűleg valahol középen van — de nem hagy nyugodni a gondolat, hogy az ágensek éjszaka dolgoztak.

---

## A. TARTALMI MINTÁK (magyar)

### 1. Túlhajtott jelentőség-tulajdonítás

**Figyelendő szavak és fordulatok:** mérföldkő, korszakalkotó, paradigmaváltó, áttöréses, úttörő szerepet játszik, kiemelt szerepet tölt be, alappillér, sarokkő, fundamentális szerepet, jelentős állomás, fontos lépés, történelmi pillanat, új fejezet, kulcsfontosságú szerep

**Probléma:** Az AI eltúlozza a téma fontosságát üres pátosszal. Magyarul ez különösen jellemző a vállalati, iparági és közigazgatási szövegekben — minden téma "új fejezetet nyit" és "kulcsszerepet tölt be".

**Előtte:**
> A digitalizációs stratégia új fejezetet nyit a vállalat életében, mérföldkő az iparág digitális átalakulásának folyamatában, és kiemelt szerepet tölt be a hosszú távú versenyképesség biztosításában.

**Utána:**
> A vállalat 2025 januárjától felhőalapú adatkezelésre vált, és három évre 12 milliárd forintot különít el a háttérrendszerek cseréjére.

---

### 2. Konkrétumok nélküli forrásmegjelölés ("homályos tekintély")

**Figyelendő fordulatok:** szakértők szerint, iparági források, egyes elemzők, a piaci szereplők, számos tanulmány, kutatások bizonyítják, általánosan elfogadott, közismert, tapasztalataink szerint

**Probléma:** Az AI vélelmezett tekintélyre hivatkozik, név és forrás nélkül. Magyarul különösen gyakori a "szakértők szerint" üres formula.

**Előtte:**
> Szakértők szerint a megújuló energia szerepe folyamatosan növekszik, és iparági források is megerősítik, hogy ez a tendencia hosszú távon fennmarad.

**Utána:**
> A MEKH 2024-es jelentése szerint a hazai szélerőműpark kapacitása 329 MW-ról 410 MW-ra nőtt 2023 és 2024 között.

---

### 3. Felszínes -ás/-és bővítmények ("látszat-mélység")

**Figyelendő fordulatok:** biztosítva ezzel..., elősegítve a..., hozzájárulva a..., lehetővé téve..., megalapozva a..., garantálva...

**Probléma:** A magyar AI-szöveg az angol "-ing" konstrukció megfelelőjeként használja a határozói igeneveket. Lánckötés helyett inkább új mondat.

**Előtte:**
> A rendszer naponta feldolgozza az adatokat, biztosítva ezzel a folyamatos áttekinthetőséget, elősegítve a gyors döntéshozatalt és hozzájárulva a hatékony működéshez.

**Utána:**
> A rendszer naponta dolgozza fel az adatokat. Így a vezetők reggel látják az előző napi forgalmat, és aznap reagálhatnak.

---

### 4. Reklámszerű, dicsérő nyelv

**Figyelendő szavak:** kiemelkedő, lenyűgöző, páratlan, egyedülálló, élvonalbeli, csúcsminőségű, prémium, innovatív, korszerű, modern, dinamikus, gazdag hagyomány, lenyűgöző természeti kincsek, festői, varázslatos, mesés

**Probléma:** A semleges leíráshoz nem szabad reklámszöveget keverni. Magyarul különösen veszélyes terület a turizmus, kultúra, és termékleírás.

**Előtte:**
> A festői Bükk-vidék szívében elhelyezkedő kisváros lenyűgöző természeti környezetével és gazdag kulturális hagyományaival élvonalbeli úti célt kínál.

**Utána:**
> A város a Bükk lábánál fekszik. Két múzeum, egy 18. századi templom és egy heti piac van benne; a környékbeli erdőkben jelölt túraútvonalak.

---

### 5. Kihívások és lehetőségek formula

**Figyelendő szerkezetek:** "Kihívások és lehetőségek", "Bár sok kihívással néz szembe...", "A nehézségek ellenére...", "A kihívások mellett a lehetőségek is megjelennek..."

**Probléma:** Az AI sablonosan illeszti ezt a szakaszt minden témához.

**Előtte:**
> A vállalat számos kihívással néz szembe a digitális átalakulás során, ugyanakkor jelentős lehetőségek is rejlenek ebben a folyamatban.

**Utána:**
> A legacy SAP-rendszer kivezetése három évig tart, és nyolc nagy üzleti folyamatot érint. A migráció miatt 2025 Q3-ban várhatóan 5–7%-os termelékenység-csökkenés lesz.

---

## B. SZÓKINCS-MINTÁK (magyar AI-szókincs)

### 6. Magas frekvenciájú magyar AI-szavak

Ezek a szavak az AI-szövegekben kiugróan gyakran fordulnak elő:

| AI-szó | Természetesebb |
|---|---|
| elengedhetetlen | szükséges, kell |
| kulcsfontosságú | fontos, lényeges |
| rendkívül | nagyon, igen, vagy hagyd el |
| kiemelkedő | jó, fontos (konkrét helyett) |
| kiemelten fontos | fontos |
| lenyűgöző | (általában elhagyandó) |
| exponenciálisan | gyorsan, sokszorosára |
| holisztikus | átfogó, teljes |
| szinergikus | együttműködő, közös |
| robusztus | stabil, megbízható, erős |
| skálázható | bővíthető, méretezhető |
| agilis | rugalmas, gyors |
| transzparens | átlátható |
| diszruptív | felforgató, áttörő |
| innovatív | új, újító |
| meghatározó | (gyakran elhagyandó) |
| alapvető | (gyakran elhagyandó) |
| dinamikus | gyors, változó |
| páratlan | (általában elhagyandó) |
| jelentős mértékben | sokat, jelentősen |

**Előtte:**
> A vállalat elengedhetetlenül fontos, kulcsfontosságú szerepet játszik a piacon, ahol kiemelkedő, innovatív és holisztikus megoldásait rendkívül dinamikusan, exponenciálisan növekvő ütemben fejleszti.

**Utána:**
> A vállalat 2024-ben 18%-kal több ügyfelet szolgált ki, mint 2023-ban. Az új szoftver három modulja idén ősszel készül el.

---

### 7. Felesleges idegen szavak

Az AI gyakran idegen tövű igéket választ, ahol van magyar megfelelő. Ez nem nyelvtisztító reflex — szakszövegben az idegen kifejezés is helyénvaló — hanem AI-jel akkor, ha **természetesebb magyar szó van helyette**.

| AI-szó | Magyar |
|---|---|
| implementál | bevezet, megvalósít |
| optimalizál | javít, finomít |
| maximalizál | növel, a legtöbbet hozza ki |
| fókuszál | összpontosít, koncentrál |
| generál | készít, létrehoz, állít elő |
| validál | ellenőriz, igazol |
| transzformál | átalakít |
| adaptál | igazít, alkalmaz |
| facilitál | elősegít, könnyít |
| monitoroz | figyel, követ |
| eskalál | továbbít, fokoz |
| prioritizál | rangsorol |
| szegmentál | feloszt, csoportosít |
| aggregál | összegez, összesít |
| eliminál | kizár, megszüntet |

**Előtte:**
> Az új rendszert 2024-ben implementáltuk, hogy optimalizáljuk az ügyfélkezelést és maximalizáljuk a hatékonyságot.

**Utána:**
> Az új rendszert 2024-ben vezettük be, hogy gyorsítsuk az ügyfélkezelést és kevesebb hibával dolgozzunk.

---

### 8. Üres töltelék-igék (verbal deflection)

A magyar AI-szöveg gyakran körülírja az egyszerű cselekvést.

| Töltelékes | Egyszerűbb |
|---|---|
| lehetőséget biztosít arra, hogy | engedi, hagyja |
| megteremti a feltételeit annak, hogy | lehetővé teszi |
| hozzájárul ahhoz, hogy | segít, miatt |
| azzal a céllal, hogy | hogy |
| abból a célból, hogy | hogy |
| annak érdekében, hogy | hogy |
| azon célból, hogy | hogy |
| abban a helyzetben van, hogy | tud, képes |
| azt eredményezi, hogy | így |
| oly módon, hogy | úgy, hogy |

**Előtte:**
> A rendszer megteremti a feltételeit annak, hogy a fejlesztők azzal a céllal dolgozzanak, hogy hozzájáruljanak a hatékonyság növeléséhez.

**Utána:**
> A rendszer segíti a fejlesztőket abban, hogy gyorsabban dolgozzanak.

---

## C. NYELVTANI ÉS MONDATSZERKEZETI MINTÁK

### 9. Bürokratikus passzív ("kerül"-mánia)

Ez a **legárulkodóbb** magyar AI-jel. A magyar nyelv ritkán használ valódi szenvedő szerkezetet, de az AI mégis tucatjával gyártja a "kerül + igenév" formulákat.

| AI-passzív | Cselekvő alak |
|---|---|
| megrendezésre kerül | megrendezzük, lesz |
| kivitelezésre kerül | kivitelezzük, megvalósítjuk |
| átadásra kerül | átadjuk, átadják |
| megtartásra kerül | megtartjuk |
| feldolgozásra kerül | feldolgozzuk |
| elfogadásra került | elfogadtuk, elfogadták |
| kihirdetésre került | kihirdették |
| végrehajtásra kerül | végrehajtjuk |
| bevezetésre kerül | bevezetjük |
| alkalmazásra kerül | alkalmazzuk, használjuk |

**Előtte:**
> A konferencia 2025 áprilisában megrendezésre kerül, ahol az új stratégia bemutatásra kerül és véleményezésre kerül a résztvevők által.

**Utána:**
> A konferenciát 2025 áprilisában tartjuk. Itt mutatjuk be az új stratégiát, és a résztvevők visszajelzést adnak rá.

---

### 10. Igekötős túlhasználat (ki-, fel-, meg-)

Az AI bizonyos igekötős igéket túl gyakran használ. Magyar fülnek "vállalati" hangulata van.

**Túlhasznált igekötős szavak:** kihangsúlyoz, kiemelten kezel, fellendít, felgyorsít, megerősít (átvitt értelemben), megalapoz, megteremt, kibővít, kibontakozik, megvalósul

**Előtte:**
> A projekt kihangsúlyozza a digitalizáció szerepét, megalapozza a hosszú távú stratégiát, fellendíti a piaci pozíciót és kibontakoztatja a versenyelőnyt.

**Utána:**
> A projekt elsődleges célja a digitalizáció. Egyben a hosszú távú stratégia alapja is, és a vállalat szerinte ezzel előzheti meg a versenytársakat.

---

### 11. "Nem X, hanem Y" parallelizmus

Magyar megfelelője az angol "It's not just X, it's Y" mintának. A pátosza miatt különösen árulkodó.

**Előtte:**
> Ez nem csupán egy szoftver, hanem egy filozófia. Nem egyszerű eszköz, hanem partner a mindennapokban. Nem csak gyors, hanem precíz is.

**Utána:**
> A szoftver három fő funkciót lát el: ügyfélkezelés, számlázás, jelentéskészítés. Naponta kétszer szinkronizál a könyveléssel.

---

### 12. Hármas szabály a magyarban

Az AI hajlamos minden gondolatot háromba csoportosítani — három jelző, három példa, három cél. Magyarul ugyanúgy árulkodó.

**Előtte:**
> A megoldás gyors, megbízható és hatékony. Csapatunk innovatív, elkötelezett és tapasztalt. A jövő digitális, fenntartható és inkluzív lesz.

**Utána:**
> A rendszer 200 ms alatt válaszol, és három éve fut hibamentesen. A csapat öt fős; mindegyikük 8+ év vállalati tapasztalattal érkezett. A középtávú terv az AWS-re költözés.

---

### 13. -ás/-és igenévhalmozás (nominalizáció)

A magyarban különösen csúnya, ha az ige helyett mindenhol főnevet használunk. AI-jel.

**Előtte:**
> A folyamat hatékonyságának növelése érdekében a rendszer újraszervezésének előkészítése és bevezetése a következő negyedév feladata.

**Utána:**
> A rendszert a következő negyedévben szervezzük újra. Először a folyamatokat mérjük fel, aztán átalakítjuk a moduláris részeit.

---

### 14. Birtokos láncok

A magyar AI hajlamos hosszú birtokos láncokat képezni: "a vállalat digitalizációjának folyamatának eredményességének kulcsa". Ez nyelvtanilag helyes lehet, de olvashatatlan.

**Szabály:** Két birtokos láncolódásnál többnél bonts mondatra.

**Előtte:**
> A digitális átalakulás folyamatának sikerességének kulcsa a vezetőség elkötelezettségének erősítésében rejlik.

**Utána:**
> A digitális átalakulás akkor sikerül, ha a vezetőség elkötelezett.

---

### 15. Halmozott "amely"-mellékmondatok

**Előtte:**
> A rendszer, amely a felhőben fut, és amelyet 2024-ben fejlesztettek, olyan funkciókat tartalmaz, amelyek a felhasználói élményt javítják.

**Utána:**
> A felhőben futó rendszert 2024-ben fejlesztettük. A felhasználói élményen több ponton javít: gyorsabb keresés, áttekinthetőbb felület, mobilbarát.

---

### 16. Túlzott magyarázó-betoldások ("ami azt jelenti, hogy")

**Előtte:**
> A latencia csökkent, ami azt jelenti, hogy a rendszer gyorsabban válaszol, ami azt eredményezi, hogy a felhasználók elégedettebbek.

**Utána:**
> A rendszer 200 ms-ról 80 ms-ra gyorsult. A felhasználók nem várnak.

---

## D. TIPOGRÁFIA ÉS FORMÁZÁS

### 17. Gondolatjel-mánia (—)

Az AI sokkal több gondolatjelet használ, mint a magyar írás megengedi. Magyar szövegben a vesszős mellékmondat vagy zárójel általában jobb választás. (A magyar tipográfia kötőjelet, nagykötőjelet és gondolatjelet különít el — az AI mindenhova nagykötőjelet vagy gondolatjelet rak.)

**Előtte:**
> A rendszer — amely 2024-ben került bevezetésre — három modult tartalmaz — beleértve az új jelentéskészítőt is — és a teljes folyamatot lefedi.

**Utána:**
> A 2024-ben bevezetett rendszer három modult tartalmaz, köztük az új jelentéskészítőt. A teljes folyamatot lefedi.

---

### 18. Idézőjel-hibák

Magyarban a helyes idézőjel **„..."** (alsó-9 nyit, felső-9 zár), nem `"..."` és nem `"..."` (curly). Az AI gyakran tévesen használja az angol formákat.

**Helyes:** „Sikeres volt a projekt", mondta a vezető.
**Helytelen:** "Sikeres volt a projekt", mondta a vezető. (curly)
**Helytelen:** "Sikeres volt a projekt", mondta a vezető. (straight, csak akkor jó, ha kódban)

---

### 19. Címek nagybetűzése (Title Case → Sentence Case)

A magyarban a címekben **csak az első szó** és a tulajdonnevek nagybetűsek. Az AI gyakran az angol Title Case-t másolja.

**Helytelen (AI):**
> ## Stratégiai Partnerségek És Globális Együttműködések

**Helyes (magyar):**
> ## Stratégiai partnerségek és globális együttműködések

---

### 20. Felkövér-halmozás

Az AI minden második kifejezést **félkövérrel** jelez. Magyar szövegben ez bántóan túltagolt.

**Előtte:**
> A **digitalizáció**, az **automatizáció** és az **AI-integráció** **kulcsfontosságú** elemei a **modern vállalati működésnek**.

**Utána:**
> A digitalizáció, automatizáció és AI-integráció a modern vállalati működés alapelemei.

---

### 21. Inline-fejléces felsorolások

**Előtte:**
> - **Felhasználói élmény:** A felület megújult.
> - **Teljesítmény:** Az algoritmusok gyorsabbak.
> - **Biztonság:** End-to-end titkosítás.

**Utána:**
> A frissítés három területet érint: új felület, gyorsabb algoritmusok, és end-to-end titkosítás.

---

### 22. Emoji a szakmai szövegben

🚀, 💡, ✅, 📊 stb. — magyar szakmai szövegbe ne kerüljön. Nem stilisztikai szabály, hanem AI-jel.

---

## E. DISKURZUS-MINTÁK ÉS SZÖVEGSTRUKTÚRA

### 23. Sablonos tudományos zárszó

**Figyelendő:** "Összegzésképpen elmondható, hogy...", "Levonható a tanulság, hogy...", "A fentiek alapján kijelenthető, hogy...", "Mindezek tükrében..."

**Előtte:**
> Összegzésképpen elmondható, hogy a digitális átalakulás kiemelkedő jelentőséggel bír, és a fentiek alapján egyértelműen kijelenthető, hogy a vállalatok számára elengedhetetlen az alkalmazkodás.

**Utána:**
> A vállalatoknak két év alatt át kell állniuk a felhőre, különben drágább lesz a karbantartás. Ezt a piacvezetők már 2023-ban elkezdték.

---

### 24. Üres szlogen-zárás

**Figyelendő:** "A jövő ígéretes", "Új korszak küszöbén állunk", "Izgalmas idők előtt állunk", "A digitális átalakulás új fejezetét nyitjuk", "Együtt egy fenntartható jövőért"

**Előtte:**
> A jövő ígéretes. Izgalmas idők előtt állunk, és együtt új korszak küszöbén lépünk át.

**Utána:**
> A következő lépés az SAP-migráció, ami 2026 januárjáig tart.

---

### 25. Üres felvezető mondatok

**Figyelendő:** "Fontos megjegyezni, hogy...", "Érdemes megemlíteni...", "Ki kell emelni...", "Nem szabad megfeledkezni arról, hogy...", "Tudni kell, hogy...", "Mielőtt belevágnánk..."

**Előtte:**
> Fontos megjegyezni, hogy a rendszer 2024-ben került bevezetésre. Érdemes megemlíteni, hogy a felhasználók pozitívan fogadták.

**Utána:**
> A rendszert 2024-ben vezettük be. A használati statisztika 30%-kal nőtt fél év alatt.

---

### 26. Chatbot-jelek

**Figyelendő:** "Természetesen!", "Persze!", "Remek kérdés!", "Igen, segítek!", "Remélem segítettem!", "Jelezz, ha bármi mást szeretnél!", "Itt egy összefoglaló..."

**Előtte:**
> Természetesen! Itt egy összefoglaló a francia forradalomról. Remélem segítettem! Jelezz, ha mást is szeretnél!

**Utána:**
> A francia forradalom 1789-ben kezdődött. A királyság pénzügyi válsága és az élelmiszerhiány robbantotta ki.

---

### 27. Szignalizáló bevezetők ("Most akkor nézzük...")

**Figyelendő:** "Most akkor nézzük...", "Vágjunk bele...", "Lássuk a részleteket...", "Most pedig...", "Mielőtt belekezdenénk..."

**Előtte:**
> Most akkor nézzük, hogyan működik a Next.js cache rendszere. Mielőtt belekezdenénk, fontos megérteni a kontextust.

**Utána:**
> A Next.js több rétegen cache-el: kérés-memoizáció, adat-cache, és router-cache.

---

### 28. Anglicizmus-fordítások

A magyar AI-szöveg angolból tükörfordított fordulatokat használ.

| Anglicizmus | Magyaros |
|---|---|
| a nap végén | végeredményben, lényegében |
| végső soron | végül, valójában |
| a táblán van | napirenden, terítéken |
| a végén a nap végén... | (ne használd kétszer!) |
| a helyzet az, hogy | (általában elhagyható) |
| így vagy úgy | valamilyen módon, akárhogy |
| a kérdés, hogy... | a kérdés az, hogy... |
| ezen a ponton | most, jelenleg |
| nézőpontból | szempontból |

**Előtte:**
> A nap végén a kérdés, hogy ezen a ponton mit tudunk csinálni. Végső soron mindenkinek a saját nézőpontból kell vizsgálni.

**Utána:**
> A kérdés most az, mit tudunk most lépni. Mindenki a saját szempontjából nézi a dolgot.

---

### 29. Túlzott mentegetőzés / kerítés ("egyfajta", "valamiféle")

**Figyelendő:** "egyfajta", "valamiféle", "egyfajta értelemben", "bizonyos mértékben", "valamilyen módon", "egyes esetekben"

**Előtte:**
> A rendszer egyfajta megoldást kínál a problémára, ami valamilyen módon bizonyos mértékben javíthatja a folyamatot.

**Utána:**
> A rendszer 30%-kal csökkenti a feldolgozási időt — méréseink szerint napi 200 tranzakciónál.

---

### 30. Ismétlő összegzés a bekezdés végén

Az AI gyakran egy bekezdés végén megismétli, amit elmondott — más szavakkal. Magyarul ez "magyarázzák a már elmagyarázottat" hatást kelt.

**Előtte:**
> A rendszer 200 ms alatt válaszol, ami nagyon gyors. Ez a sebesség azt jelenti, hogy a felhasználóknak nem kell várniuk, és így gyorsan tudnak dolgozni.

**Utána:**
> A rendszer 200 ms alatt válaszol. A felhasználók nem várnak rá.

---

## Folyamat

1. **Olvasd el a teljes szöveget.** Mi a célja, kihez szól, milyen regiszterben?
2. **Ha van hangminta, elemezd azt először.**
3. **Azonosítsd a mintákat.** Listázd, ne írj át mindent vakon.
4. **Készíts egy első átírást.** Tartsd meg a tartalmat, cseréld a formát.
5. **Audit kérdés:** "Mitől hangzik még mindig AI-szerűnek?"
6. **Válaszolj röviden** a maradék jelekre.
7. **Készíts egy második átírást** az audit alapján.
8. **Mutasd meg mindkét verziót** és a változtatások listáját.

## Kimeneti formátum

1. **Első átírás** (Draft)
2. **"Mitől AI-szerű még?"** (rövid lista)
3. **Végső változat** (Final)
4. **Változtatások** (opcionális, rövid összefoglaló)

---

## Teljes példa

**Előtte (AI-magyar):**

> Természetesen! Az AI-asszisztált kódolás kiemelkedő mérföldkő a szoftverfejlesztés evolúciójának folyamatában, és kulcsfontosságú szerepet tölt be a modern technológiai környezet alakításában. Ezek az úttörő eszközök — amelyek a kutatás és a gyakorlat metszéspontjában helyezkednek el — alapvetően átalakítják a fejlesztők munkáját, kihangsúlyozva a digitális átalakulás jelentőségét.
>
> Lényegében a hozzáadott érték egyértelmű: a folyamatok optimalizálása, az együttműködés elősegítése és a koordináció maximalizálása. Nem csupán egy autocomplete eszköz, hanem egy partner. Nem egyszerűen kódot generál, hanem inspirál.
>
> A bevezetés exponenciálisan gyorsult fel a hobbifejlesztőktől a vállalati körökig, a független fejlesztőktől a cross-funkcionális csapatokig. Iparági források szerint a technológia rendkívül innovatív, és holisztikus megközelítést kínál.
>
> - 💡 **Sebesség:** A kódgenerálás kerül felgyorsításra, jelentős mértékben csökkentve a súrlódást.
> - 🚀 **Minőség:** A kimeneti minőség javításra kerül, hozzájárulva a magasabb sztenderdekhez.
> - ✅ **Elfogadás:** A használat folyamatosan növekszik.
>
> Bár a részletek korlátozottan állnak rendelkezésre, egyfajta értelemben kijelenthető, hogy az eszközök bizonyos mértékben pozitív hatást gyakorolnak. A kihívások ellenére — beleértve a hallucinációkat, az elfogultságot és a felelősségvállalást — az ökoszisztéma virágzik. Annak érdekében, hogy a teljes potenciál kibontakozhasson, a csapatoknak alkalmazkodniuk kell a legjobb gyakorlatokhoz.
>
> Összegzésképpen elmondható, hogy a jövő ígéretes. Izgalmas idők előtt állunk a kiválóság felé vezető úton. Remélem, hasznos volt!

**Első átírás:**

> Az AI-kódolóasszisztensek néhány feladatban gyorsabbá teszik a fejlesztőt. Egy 2024-es Google-vizsgálat szerint a Codex-felhasználók 55%-kal hamarabb írtak meg egyszerű függvényeket, mint a kontrollcsoport. Hibakeresésben és architekturális döntéseknél nem volt kimutatható különbség.
>
> Az eszközök jól dolgoznak boilerplate-en: konfigfájlok, teszt-vázak, ismétlődő refaktorok. Rosszul ismerik fel, mikor tévednek. Én is elfogadtam már olyan javaslatokat, amelyek lefordultak, átmentek a linten, és mégis mást csináltak, mert egy ponton abbahagytam a figyelést.
>
> Két táborra szakad a fejlesztői közösség. Egyik fele autocomplete-ként használja unalmas kódra, és minden sort ellenőriz. A másik kikapcsolja, miután kétszer is javasolt egy elavult belső könyvtárat.
>
> A produktivitási számok ingatagok. A GitHub szerint a Copilot-felhasználók "30%-ban elfogadják a javaslatokat" — de az elfogadás nem egyenlő a helyességgel, és a helyesség nem egyenlő az értékkel. Az Uplevel 2024-es tanulmánya nem talált statisztikailag szignifikáns különbséget a PR-átfutásban AI-asszisztált és nem asszisztált csapatok között.
>
> Nem haszontalanok az eszközök — csak eszközök. Nem helyettesítik az ítélőképességet, és nem váltják ki a teszteket. Tesztek nélkül nem tudod megmondani, jó-e a javaslat.

**Mitől AI-szerű még?**
- A bekezdések túl rendezettek, mindegyik kis tanulsággal zár.
- A "Két táborra szakad..." kicsit kerek, sablonos összefoglaló.
- A záró mondat ("Tesztek nélkül nem tudod megmondani...") szlogenes.

**Végső változat:**

> Az AI-kódoló jó dolgokra jó. Boilerplate-re, konfigfájlra, teszt-vázra. Nem architektúrára. Pláne nem a hajnali deploy közbeni vészhelyzetre.
>
> A baj az, hogy ami jónak tűnik, nem feltétlenül jó. Volt, hogy egy egész napon át fogadtam el javaslatokat, lefordultak, lintelt is — aztán kiderült, hogy a függvényt rosszul hívtam, csak nem szólt érte semmi. A modell magabiztos volt. Én megbíztam benne.
>
> Olyan emberekkel beszéltem, akik szeretik. És olyanokkal, akik kikapcsolták, mert a Copilot folyamatosan egy elavult belső könyvtárat ajánlgatott. Mindkettőt értem.
>
> Egy szám van, ami fennakadt nálam: az Uplevel 2024-es vizsgálata szerint AI-val és AI nélkül **nem volt** statisztikailag mérhető különbség a PR-átfutásban. Ez nem azt jelenti, hogy az eszköz haszontalan. Azt jelenti, hogy az „elfogadási arány" meg az „elégedettség" nem ugyanaz, mint a kibocsátás.
>
> Tesztek nélkül egyébként is sötétben tapogatózol — Copilottal vagy nélküle.

**Változtatások:**
- Eltávolítva: chatbot-felvezető ("Természetesen!"), zárás ("Remélem hasznos volt!")
- Eltávolítva: pátoszos szókincs (mérföldkő, kulcsfontosságú, úttörő, exponenciálisan, holisztikus, rendkívül)
- Eltávolítva: "kerül"-passzív (felgyorsításra kerül, javításra kerül)
- Eltávolítva: "Nem X, hanem Y" parallelizmus (nem csupán autocomplete...)
- Eltávolítva: hármas-szabály felsorolások (folyamatok / együttműködés / koordináció)
- Eltávolítva: emojik, félkövér fejlécek, gondolatjelek
- Eltávolítva: homályos forrás ("Iparági források szerint")
- Eltávolítva: kerítés-szavak ("egyfajta értelemben", "bizonyos mértékben")
- Eltávolítva: sablonos zárás ("a jövő ígéretes", "izgalmas idők előtt állunk")
- Cserélt: "annak érdekében, hogy" → "hogy"
- Cserélt: birtokos láncok feloldva
- Hozzáadva: konkrét adat (Uplevel 2024), saját első személyű tapasztalat, tagadás-érv (nem volt különbség), enyhe humor (hajnali deploy)

---

## Hivatkozás

A skill az alábbi forrásokra épül:
- [blader/humanizer](https://github.com/blader/humanizer) — angol minták
- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) — alapminták
- Magyar nyelvi tapasztalat — magyar-specifikus minták

A magyar adaptáció kiegészítései a `references/` mappában találhatók:
- `references/szokincs.md` — kibővített AI-szókincs lista magyar megfelelőkkel
- `references/tipografia.md` — magyar tipográfiai szabályok
- `references/peldak.md` — további részletes átírási példák

Kulcsmeglátás (Wikipedia): "Az LLM-ek statisztikai algoritmussal találgatják, mi következik. Az eredmény a legvalószínűbb válasz felé mutat, ami a legtöbb esetre alkalmazható." Magyarul: az AI-szöveg az átlag felé húz, a humanizálás pedig a konkrétumok és a személyes hang felé.
