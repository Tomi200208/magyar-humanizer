# Magyar tipográfia — humanizer-szempontból

A tipográfiai jeleket az AI gyakran helytelenül használja. Néhány eltérés a magyar és angol szabályok között:

## 1. Idézőjelek

**Helyes magyar:** „idézet" — alsó-9 (U+201E) nyit, felső-9 (U+201D) zár.

**Másodlagos idézőjel** (idézet az idézetben): »idézet a magyar idézőjelben« — francia (»...«) jelek.

**Helytelen (de gyakori AI-hiba):**
- "idézet" (curly, angol) — tipikus AI-jel
- "idézet" (egyenes) — csak kódban indokolt
- 'idézet' (aposztróf) — tipográfiai hiba

**Példa:**
- ✅ A vezető szerint „a projekt sikeres lett".
- ❌ A vezető szerint "a projekt sikeres lett". (curly)
- ❌ A vezető szerint "a projekt sikeres lett". (straight)

## 2. Gondolatjel, nagykötőjel, kötőjel

A magyar tipográfia **három** dash-típust különböztet meg:

### Kötőjel (-) — U+002D
Szóösszetétel, toldalékolás:
- AI-asszisztens
- TechCorp-csoport
- 2024-ben

### Nagykötőjel (–) — U+2013
Tartomány, viszony, kapcsolat (szóközök nélkül):
- 2024–2025
- 10–20 fő
- Budapest–Bécs vonal
- Anglia–Magyarország mérkőzés

### Gondolatjel (—) — U+2014 vagy nagykötőjel-szóközös változata (– space – space)
Mondatközi közbevetés. Itt a magyar tipográfia ingadozik:
- A klasszikus szabály: nagykötőjel szóközökkel: " – "
- A modern, számítógépes gyakorlat: gondolatjel szóközökkel: " — "
- Mindkettő elfogadott, de **válassz egyet és tartsd**.

**AI-hiba:** túl sok közbevetés, és gyakran helytelen kötőjelet használ.

**Példa:**
- ✅ A rendszer – amelyet 2024-ben vezettünk be – jól működik.
- ✅ A rendszer — amelyet 2024-ben vezettünk be — jól működik.
- ❌ A rendszer-amelyet 2024-ben vezettünk be-jól működik. (kötőjel, helytelen)

**Humanizer-szabály:** Ha 2-nél több gondolatjel van egy bekezdésben, valószínűleg cserélni kell vesszőre vagy zárójelre.

## 3. Címek nagybetűzése

Magyar címben **csak az első szó és a tulajdonnév nagybetűs**.

**Helyes:**
- Stratégiai partnerségek és nemzetközi együttműködések
- A digitalizáció szerepe a magyar energetikában
- Az X Vállalat innovációs portfóliója

**Helytelen (Title Case, AI-jel):**
- Stratégiai Partnerségek És Nemzetközi Együttműködések
- A Digitalizáció Szerepe A Magyar Energetikában

## 4. Számok és mértékegységek

### Tizedesjel
- Magyar: vessző — 3,14
- Angol: pont — 3.14
- AI-hiba: pont magyar szövegben

### Ezres elválasztó
- Magyar: szóköz vagy pont — 1 234 567 vagy 1.234.567
- Angol: vessző — 1,234,567
- AI-hiba: vessző magyar szövegben

### Százalékjel
- Magyar: szóközzel — 25 %
- De a szakmai gyakorlat sokszor: 25%
- Mindkettő elfogadott, de **következetes legyen**.

### Mértékegységek
- Magyar: szóközzel — 5 km, 10 kg, 230 V
- Pénznem: Magyarországon a "Ft" áll a szám után — 1000 Ft (szóközzel)
- AI-hiba: $ jel keverése magyar szövegbe

## 5. Toldalékolt rövidítések

Rövidítésekhez kötőjellel kapcsoljuk a toldalékot:
- ✅ KSH-tól, NAV-tól, USA-ban, EU-ban
- ❌ KSH-tól (helyes), KSHtól (helytelen), KSH tól (AI-hiba)

**Speciális esetek:**
- Mozaikszó kis betűkkel: nato-tag → NATO-tag (ha ismert mozaikszó, csupa nagy)
- Mértékegység után: 5 km-en, 10 kg-tól

## 6. Felsorolás-jelek

### Bullet point
- Magyar: kötőjel (–) vagy bullet (•)
- Az AI gyakran csillag-bullet (★, ✦), emoji-bullet (✅, 🔹) — ezek AI-jelek

### Számozott felsorolás
- Magyarban gyakran 1., 2., 3. (ponttal)
- Az AI néha "1)" formát használ — angol stílus

## 7. Bekezdés-formázás

### Behúzás
- Tipikus magyar könyvbeli stílus: első sor behúzott, sortávolság kicsi
- Hivatalos / vállalati: nincs behúzás, sortávolság nagyobb (Word-stílus)
- Az AI általában a Word-stílust követi — ez magyar környezetben is elfogadott

### Bekezdés-hossz
- Magyar AI-szöveg jellemzője: minden bekezdés 4-5 sor, egyenletes
- Természetes szöveg: változó, néha 1 mondat, néha 10
- **Humanizer-szabály:** ha minden bekezdés ugyanolyan hosszú, vágj bele.

## 8. Felkövér és dőlt

### Félkövér (bold)
- Magyar szakmai szövegben: címek, kulcsfogalmak első előfordulása
- Az AI mindenhol kiemel — ez túltagolt

**Szabály:** ha 5 mondatban 3+ félkövér kifejezés van, törölni kell a felét.

### Dőlt (italic)
- Magyar használat: idegen szavak, könyvcímek, finom hangsúly
- Az AI ritkán dőlt — inkább félkövér; ezért a sok félkövér tipikus AI-jel

## 9. Idegen szavak helyesírása

A magyarban az idegen szavakat **kiejtés szerint vagy eredeti írás szerint** írjuk, és ennek szabálya van:

### Eredeti írás (gyakran a szakmai szövegben)
- software → software (informatikai szövegben sokszor megmarad)
- AI, IT, CEO, KPI

### Magyaros írás
- szoftver (köznyelvi)
- számítógép (helyett: computer)

**AI-jel:** keveredés ugyanazon a szövegen belül. Maradj egy verziónál.

## 10. Idézet központozása

Az idézőjel utáni mondatzáró pont szabálya **eltér** az angol és magyar gyakorlatban:

### Magyar
- A pont **az idézőjelen kívülre** kerül, ha a mondat folytatódik vagy az idézet részmondat:
  - A vezető azt mondta: „a projekt sikerült".
- A pont **az idézőjelen belül** marad, ha az idézet teljes mondat:
  - „A projekt sikerült." Ezt mondta a vezető.

### Angol
- A pont általában az idézőjelen belül.

**AI-jel:** angol szabályú központozás magyar szövegben.

## 11. Címsor-szabályok (markdown és Word)

### H1, H2, H3...
- **AI-jel:** felülről lefelé hierarchia helyett vízszintes ismétlés (5 db H2 ugyanarról).
- **AI-jel:** minden bekezdés előtt H3 — túltagolt.
- **Természetes:** kevés címsor, hosszabb prózás szakaszok.

### Címsor-szöveg
- Sentence case (csak első szó nagy)
- Rövid, leíró
- Nincs benne emoji
- Nincs benne kérdőjel-felkiáltójel

## 12. Linkek és hivatkozások

### Magyar tudományos / szakmai szövegben
- Lábjegyzet-szám felső indexben¹
- Vagy zárójeles hivatkozás: (Kovács, 2024)
- AI-jel: [link szöveg](url) markdown formátum keveredése prózás szövegbe

### Webes / blog-jellegű
- Inline link természetes
- AI-jel: minden mondatban link, túldokumentált

## Összefoglaló: a leggyakoribb AI tipográfiai hibák magyar szövegben

1. **Curly idézőjel** "..." `„..."` helyett — szinte mindig AI-jel
2. **Title Case címek** — Stratégiai Partnerségek
3. **Túl sok félkövér** kifejezés egy bekezdésben
4. **Túl sok gondolatjel**-es közbevetés
5. **Tizedespont** vessző helyett
6. **Emoji** szakmai szövegben
7. **Vesszős ezres elválasztó** (1,234) szóköz helyett
8. **Toldalékolatlan rövidítések** ("KSH-tól" helyett "KSHtól" vagy "KSH tól")
9. **Egyenletes bekezdéshossz** (mindegyik 4 sor)
10. **Sűrű címsor-hierarchia** — minden 3-4 mondat után új cím
