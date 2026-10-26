# Online vektorový editor

**Autor:** Lucia Benovicsová  
**Školiteľ:** doc. PaedDr. Monika Tomcsányiová, PhD.

## Zadanie práce

Online vektorový editor bude mať implementované základné nástroje vektorových editorov, ako je kreslenie geometrických útvarov, úprava útvarov pomocou ťahania bodov a práca s vrstvami.

Nástroje budú upravené tak, aby boli intuitívne pre detského používateľa. Súčasťou aplikácie bude import a export nakreslených obrázkov v bežnom vektorovom formáte.

Spôsob implementácie programu bude vyplývať z analýzy vývojových nástrojov a rozhodnutia autora záverečnej práce. Aplikácia bude vyvíjaná pomocou metodológie **Design-Based Research (DBR)**, ktorá je založená na prepojení potrieb pedagogického výskumu a reality v triede.

Vďaka viacnásobnému testovaniu aplikácie so žiakmi bude možné vytvoriť softvér, ktorý sa bude dať využívať v školskej praxi.

## Ciele diplomovej práce

Hlavným cieľom diplomovej práce je navrhnúť a implementovať online vektorový editor, ktorý umožňuje používateľom vytvárať, upravovať a zdieľať vektorovú grafiku priamo vo webovom prehliadači.

Súčasťou riešenia je aj podpora kolaboratívneho kreslenia v reálnom čase prostredníctvom zdieľaných miestností.

### Čiastkové ciele

- Analyzovať existujúce riešenia online vektorových editorov a kolaboratívnych nástrojov.
- Navrhnúť architektúru webovej aplikácie.
- Implementovať používateľské rozhranie vektorového editora s nástrojmi na kreslenie a úpravu základných vektorových objektov.
- Zabezpečiť prácu s objektmi na kresliacej ploche.
- Implementovať export a import vytvorenej kresby, napríklad vo formáte JSON a PNG.
- Navrhnúť a implementovať zdieľané miestnosti, do ktorých sa používatelia môžu pripájať pomocou unikátneho identifikátora.
- Zabezpečiť synchronizáciu zmien medzi viacerými používateľmi v reálnom čase pomocou WebSocket komunikácie.
- Otestovať funkčnosť aplikácie pri lokálnom použití a pri súčasnej práci viacerých používateľov v jednej miestnosti pomocou techník DBR.
- Implementovať zmeny pomocou analýzy priebehu testovania podľa DBR.

## Použité technológie

### Frontend

- React
- Vite
- JavaScript
- HTML
- CSS
- SVG

### Backend

- Node.js
- Express
- Socket.IO

### Ďalšie technológie

- WebSocket komunikácia prostredníctvom Socket.IO
- Git a GitHub
- Vercel – nasadenie frontendovej časti
- Render – nasadenie backendovej časti

# Priebežný progres

## Február 2026

- Analýza existujúcich riešení vektorových editorov.
- Analýza podobných online nástrojov.

## Marec 2026

- Hľadanie a štúdium vedeckých článkov.
- Štúdium metodológie Design-Based Research.

## Apríl 2026

- Vytvorenie prvého funkčného prototypu vektorového editora.
- Implementácia základnej kresliacej plochy a jej funkcionalít.

## Máj 2026

- Návrh kolaboratívnej časti aplikácie.
- Vytvorenie miestností so 4-ciferným ID.
- Implementácia synchronizácie kresby medzi používateľmi v reálnom čase pomocou Socket.IO.

## Jún 2026 – testovanie aplikácie

### 1. testovanie – 9. 6. 2026

- 2 testeri, vo dvojici
- zameranie na základné funkcie a kolaboratívne kreslenie

**Zistené chyby:**

- problémy s priehľadnosťou tvarov,
- rozdielny výber farieb v rôznych webových prehliadačoch,
- chýbajúca funkcionalita klávesu Shift pri kreslení štvorca, kruhu a rovnej čiary,
- nefungujúce klávesové skratky CTRL+Z a CTRL+Y,
- problém s kolíziami – pri práci jedného používateľa bola druhému zablokovaná funkcionalita editora.

### 2. testovanie – 22. 6. 2026

- testovanie v triede,
- 5. ročník ZŠ,
- 14 testerov,
- testovanie v prirodzenom prostredí bez priamej pomoci,
- pripravené 3 úlohy zamerané na samostatnú prácu aj spoluprácu.

**Zistené chyby a chýbajúce funkcie:**

- chýba nástroj na kreslenie rovnej čiary,
- chýba klávesová skratka CTRL+D,
- chýba možnosť pridávať text,
- nejasné potvrdenie vstupu do miestnosti,
- chýbajú mená používateľov pri editovaní objektov.

## September 2026

Aplikácia bola ďalej rozšírená a pripravená na ďalšie testovanie.

Boli upravené najmä funkcie súvisiace s kolaboráciou a súčasnou prácou viacerých používateľov. Postupne boli pridané používateľské mená a upravené riešenie kolízií pri práci s rovnakými objektmi.

Aplikácia bola následne pripravená na testovanie so žiakmi 9. ročníka.

## September – október 2026 – testovanie so žiakmi

Aplikácia bola testovaná triedou žiakov 9. ročníka.  
Cieľom bolo sledovať prácu žiakov s editorom, overiť zrozumiteľnosť jednotlivých nástrojov a získať spätnú väzbu na ďalší vývoj.

Na základe testovania boli identifikované najmä tieto požiadavky a nedostatky:

- chýba nástroj na kreslenie rovných čiar,
- nie je možné vybrať viac objektov naraz,
- chýba možnosť vypnúť obrys objektu,
- problémy s výberom a vypĺňaním farieb v niektorých prehliadačoch,
- požiadavka na úpravu gumy tak, aby bolo možné vymazať iba časť nakreslenej čiary,
- požiadavka na väčšie možnosti deformácie objektov.

Táto spätná väzba bola použitá pri ďalšej iterácii vývoja podľa metodológie DBR.

## Október 2026

Počas októbra pokračovalo ďalšie vylepšovanie aplikácie a zároveň sme sa začali intenzívnejšie venovať písomnej časti diplomovej práce.

Postupne sme:

- začali spracovávať kapitolu Analýza problematiky,
- čítali a spracovávali odborné a vedecké články,
- hľadali ďalšie zdroje zamerané na edukačný softvér, používateľské rozhranie, kolaboratívne učenie a Design-Based Research,
- upravovali spôsob citovania a bibliografické záznamy jednotlivých zdrojov,
- pokračovali v testovaní aplikácie,
- priebežne zapracovávali výsledky testovaní do ďalších verzií softvéru.

Vývoj aplikácie a písanie diplomovej práce tak v tomto období prebiehali paralelne.

### 5. testovanie – 9. 10. 2026

Testovanie prebehlo v dvojici a bolo zamerané najmä na overenie kolaboratívnych funkcií po ich úprave.

V tejto verzii aplikácie už boli:

- pridané používateľské mená,
- upravené zobrazovanie používateľov pri práci s objektmi,
- vyriešené základné kolízie pri súčasnej práci viacerých používateľov.

Počas testovania sme sledovali najmä prácu dvoch používateľov v jednej miestnosti a správanie aplikácie pri súčasnom kreslení a úprave objektov.

**Zistené chyby a problémy:**

- CTRL+Z a CTRL+Y nefungovali správne iba nad vlastnými krokmi používateľa,
- bolo potrebné upraviť históriu zmien tak, aby používateľ nemohol vrátiť zmenu vykonanú druhým používateľom,
- objavil sa problém pri práci so štvoruholníkom,
- pri niektorých čiarach nebolo možné objekt označiť kliknutím do jeho vnútornej časti.

Testovanie ukázalo, že základné problémy s kolaboráciou a kolíziami sa podarilo výrazne zlepšiť. Ďalšie úpravy bolo potrebné zamerať najmä na históriu zmien a správne označovanie objektov.

### 6. testovanie – 19. 10. 2026

- testovanie v triede 4. ročníka ZŠ,
- 24 testerov,
- testovanie v prirodzenom školskom prostredí,
- spätná väzba získavaná najmä pozorovaním priebehu hodiny,
- úlohy boli zamerané na samostatnú prácu aj kolaboráciu,
- pred začiatkom neprebehla rozsiahla demonštrácia aplikácie,
- žiaci dostávali iba menšiu pomoc v prípadoch, keď si nevedeli rady.

Cieľom bolo sledovať, ako intuitívne dokážu aplikáciu používať mladší žiaci a či dokážu pochopiť jednotlivé nástroje aj bez predchádzajúcich skúseností s vektorovými editormi.

**Zistenia a spätná väzba:**

- žiaci 4. ročníka ešte nemali veľa skúseností so štandardnými grafickými editormi,
- menej poznali princípy ako používanie klávesu Shift, označovanie objektov alebo práca s výplňou,
- pri niektorých funkciách preto potrebovali krátke vysvetlenie,
- kolaboratívna práca fungovala bez výraznejších problémov,
- spoločné kreslenie žiakov bavilo a aktívne túto možnosť využívali,
- princíp vrstiev pre väčšinu žiakov nebol zo začiatku známy, ale po krátkom vysvetlení ho pochopili,
- pri ostatných základných funkciách sa nevyskytli výraznejšie problémy.

Testovanie ukázalo, že aplikácia je použiteľná aj pre mladších žiakov, ktorí ešte nemajú skúsenosti s bežnými vektorovými editormi. Zároveň sa ukázalo, že funkcie, ktoré sú pre skúsenejšieho používateľa štandardné, nemožno pri mladších žiakoch automaticky považovať za známe. Pri ďalšom návrhu aplikácie a používateľskom testovaní je preto potrebné túto skutočnosť zohľadniť.

# Aktuálne funkcie aplikácie

Aplikácia v súčasnosti podporuje:

- vytvorenie spoločnej miestnosti,
- pripojenie do miestnosti pomocou ID,
- používateľské mená,
- kolaboratívne kreslenie v reálnom čase,
- synchronizáciu zmien medzi používateľmi,
- informáciu o tom, ktorý používateľ má označený objekt,
- riešenie súčasnej práce viacerých používateľov s objektmi,
- kreslenie geometrických útvarov,
- kreslenie voľnou rukou,
- výber a presúvanie objektov,
- úpravu objektov,
- zmenu výplne a obrysu,
- zmenu hrúbky čiary,
- mazanie,
- prácu s vrstvami,
- skrývanie a zobrazovanie objektov,
- Undo/Redo,
- zoom,
- import a export projektu,
- online používanie aplikácie prostredníctvom webového prehliadača.

# Plánované úlohy

Na základe posledných testovaní sú plánované najmä tieto úpravy:

- oprava Undo/Redo pri kolaboratívnom používaní tak, aby používateľ pracoval iba s vlastnou históriou zmien,
- oprava označovania čiar a ďalších objektov,
- implementácia nástroja na kreslenie rovnej čiary,
- výber viacerých objektov naraz,
- úprava gumy tak, aby bolo možné odstrániť iba časť nakreslenej čiary,
- rozšírenie možností deformácie objektov,
- možnosť vypnúť obrys objektu,
- ďalšie zlepšenie používateľského rozhrania,
- oprava problémov súvisiacich s rozdielnym správaním webových prehliadačov,
- ďalšie testovanie aplikácie,
- analýza výsledkov testovania podľa DBR,
- zapracovanie výsledkov testovania do diplomovej práce,
- pokračovanie v štúdiu vedeckých článkov,
- dokončenie písomnej časti diplomovej práce.

# Architektúra aplikácie

Aplikácia je rozdelená na dve hlavné časti:

**Frontend** predstavuje samotný vektorový editor, s ktorým pracuje používateľ vo webovom prehliadači. Je vytvorený pomocou React a Vite.

**Backend** zabezpečuje komunikáciu medzi používateľmi a správu kolaboratívnych miestností. Je vytvorený pomocou Node.js, Express a Socket.IO.

Pri kolaboratívnom kreslení sa zmena vykonaná jedným používateľom odošle na server a následne sa synchronizuje s ostatnými používateľmi pripojenými do rovnakej miestnosti.

```markdown
# Vedecké články a zdroje

Pri spracovaní teoretickej časti diplomovej práce a pri návrhu metodiky vývoja aplikácie používame najmä zdroje zamerané na edukačný softvér, používateľské rozhranie, kognitívnu záťaž a metodológiu Design-Based Research.

## Design-Based Research

- **Armstrong, M., Dopp, C., Welsh, J. – Design-Based Research (2020)**  
  Kapitola z publikácie *The Students' Guide to Learning Design and Research*. Zdroj používame najmä na základné vysvetlenie metodológie Design-Based Research a jej využitia pri návrhu a postupnom overovaní riešenia.  
  [https://edtechbooks.org/studentguide/design-based_research](https://edtechbooks.org/studentguide/design-based_research)

- **Barab, S. A., Squire, K. – Design-Based Research: Putting a Stake in the Ground (2004)**  
  Článok sa venuje charakteristike Design-Based Research a jeho využitiu pri výskume vzdelávacích riešení v reálnom prostredí.  
  [https://www.researchgate.net/publication/213801788_Design-Based_Research_Putting_a_Stake_in_the_Ground](https://www.researchgate.net/publication/213801788_Design-Based_Research_Putting_a_Stake_in_the_Ground)

- **Sousa, L., Pedro, L., Santos, C. – An Introduction to Design-Based Research in TEL**  
  Zdroj sa venuje využitiu Design-Based Research v oblasti Technology Enhanced Learning a jednotlivým fázam tejto metodológie.  
  [https://ea-tel.eu/detel-book/chapter/methodologies/design-based-research/](https://ea-tel.eu/detel-book/chapter/methodologies/design-based-research/)

- **The Design-Based Research Collective – Design-Based Research: An Emerging Paradigm for Educational Inquiry (2003)**  
  Jeden zo základných zdrojov metodológie Design-Based Research. Článok opisuje prepojenie návrhu vzdelávacieho riešenia, jeho skúmania a postupného upravovania na základe získaných výsledkov.  
  [https://www.researchgate.net/publication/258028835_Design-Based_Research_An_Emerging_Paradigm_for_Educational_Inquiry](https://www.researchgate.net/publication/258028835_Design-Based_Research_An_Emerging_Paradigm_for_Educational_Inquiry)

- **Wang, F., Hannafin, M. J. – Design-Based Research and Technology-Enhanced Learning Environments (2005)**  
  Článok sa venuje využitiu Design-Based Research pri návrhu technologicky podporovaných vzdelávacích prostredí. Tento zdroj je pre našu prácu dôležitý najmä kvôli prepojeniu návrhu softvéru, jeho testovania v reálnom prostredí a následných iteratívnych úprav.  
  [https://www.researchgate.net/publication/225626676_Design-based_research_and_technology-enhanced_learning_environments](https://www.researchgate.net/publication/225626676_Design-based_research_and_technology-enhanced_learning_environments)

## Edukačný softvér a používateľské rozhranie

- **Sim, G., MacFarlane, S., Read, J. – All Work and No Play: Measuring Fun, Usability, and Learning in Software for Children (2006)**  
  Článok skúma použiteľnosť, zábavnosť a efekt učenia pri edukačnom softvéri určenom deťom. Používame ho najmä pri spracovaní vlastností edukačného softvéru a jeho používateľského testovania.  
  [https://www.tlu.ee/~kpata/haridustehnoloogiaTLU/funusability.pdf](https://www.tlu.ee/~kpata/haridustehnoloogiaTLU/funusability.pdf)

- **Taibah, M. A. – Usability Survey of Educational Software Used by Children at Schools (2016)**  
  Zdroj sa zaoberá použiteľnosťou edukačného softvéru v školskom prostredí a špecifikami detských používateľov. V našej práci ho využívame najmä pri opise edukačného softvéru, používateľského rozhrania a potreby testovania aplikácie na cieľovej skupine.  
  [https://journals.gmu.edu/jmgr/article/view/530](https://journals.gmu.edu/jmgr/article/view/530)

- **Mayer, R. E., Moreno, R. – Nine Ways to Reduce Cognitive Load in Multimedia Learning (2003)**  
  Článok sa venuje kognitívnej záťaži pri multimediálnom učení. V našej práci ho využívame najmä pri návrhu jednoduchého a zrozumiteľného používateľského rozhrania, ktoré používateľa zbytočne nezaťažuje nadbytočnými prvkami.  
  [https://www.researchgate.net/publication/253772914_Nine_Ways_to_Reduce_Cognitive_Load_in_Multimedia_Learning](https://www.researchgate.net/publication/253772914_Nine_Ways_to_Reduce_Cognitive_Load_in_Multimedia_Learning)


# Materiály

- [Spustiteľná online verzia aplikácie](https://online-vektorovy-editor.vercel.app/)
- [Písomná časť diplomovej práce](diplomovka-1.pdf)
- [Prezentácia pokroku](ONLINE%20VEKTOROV%C3%9D%20EDITOR.pptx)
- [Aktuálna verzia aplikácie](vector_editor.zip)
- [Zdrojové kódy aplikácie](DOPLNIŤ_ODKAZ)
- [Použité knižnice a technológie](DOPLNIŤ_ODKAZ)
- [Materiály k testovaniu](DOPLNIŤ_ODKAZ)
```

## Aktuálny stav projektu

V súčasnosti je vytvorená **funkčná online verzia kolaboratívneho vektorového editora**. Aplikácia umožňuje viacerým používateľom pripojiť sa do spoločnej miestnosti a pracovať na jednej kresbe v reálnom čase.

Aplikácia už prešla viacerými iteráciami testovania. Testovanie prebehlo v dvojiciach aj v reálnom školskom prostredí so žiakmi rôznych vekových skupín. Posledné testovanie prebehlo v triede 4. ročníka ZŠ s 24 žiakmi a bolo zamerané najmä na intuitívnosť ovládania a kolaboratívnu prácu.

Na základe získanej spätnej väzby pokračuje ďalšia iterácia vývoja, ktorej cieľom je odstrániť zostávajúce nedostatky a upraviť aplikáciu podľa potrieb cieľových používateľov.

Súčasne pokračuje písanie diplomovej práce, štúdium vedeckých článkov a spracovanie teoretických východísk, najmä v oblasti edukačného softvéru a metodológie Design-Based Research.

## Súbory v repozitári

- [Písomná časť diplomovej práce](diplomovka-1.pdf)
- [Prezentácia pokroku](ONLINE%20VEKTOROV%C3%9D%20EDITOR.pptx)
- [Aktuálna verzia aplikácie](vector_editor.zip)
