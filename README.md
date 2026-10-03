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

- problémy s priehľadnosťou tvarov
- rozdielny výber farieb v rôznych webových prehliadačoch
- chýbajúca funkcionalita klávesu Shift pri kreslení štvorca, kruhu a rovnej čiary
- nefungujúce klávesové skratky CTRL+Z a CTRL+Y
- problém s kolíziami – pri práci jedného používateľa bola druhému zablokovaná funkcionalita editora

### 2. testovanie – 22. 6. 2026

- testovanie v triede
- 5. ročník ZŠ
- 14 testerov
- testovanie v prirodzenom prostredí bez priamej pomoci
- pripravené 3 úlohy zamerané na samostatnú prácu aj spoluprácu

**Zistené chyby a chýbajúce funkcie:**

- chýba nástroj na kreslenie rovnej čiary
- chýba klávesová skratka CTRL+D
- chýba možnosť pridávať text
- nejasné potvrdenie vstupu do miestnosti
- chýbajú mená používateľov pri editovaní objektov
- 

## September 2026

Aplikácia bola ďalej rozšírená a pripravená na ďalšie testovanie.

Aplikácia bola následne pripravená na testovanie so žiakmi 9. ročníka.

## September – október 2026 – testovanie so žiakmi

Aplikácia bola testovaná triedou žiakov 9. ročníka. 
Cieľom bolo sledovať prácu žiakov s editorom, overiť zrozumiteľnosť jednotlivých nástrojov a získať spätnú väzbu na ďalší vývoj.

Na základe testovania boli identifikované najmä tieto požiadavky a nedostatky:

- chýba nástroj na kreslenie rovných čiar,
- nie je možné vybrať viac objektov naraz,
- chýba možnosť vypnúť obrys objektu.

Táto spätná väzba bude použitá pri ďalšej iterácii vývoja podľa metodológie DBR.

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

Na základe posledného testovania sú plánované najmä tieto úpravy:

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
- dokončenie písomnej časti diplomovej práce.


# Architektúra aplikácie

Aplikácia je rozdelená na dve hlavné časti:

**Frontend** predstavuje samotný vektorový editor, s ktorým pracuje používateľ vo webovom prehliadači. Je vytvorený pomocou React a Vite.

**Backend** zabezpečuje komunikáciu medzi používateľmi a správu kolaboratívnych miestností. Je vytvorený pomocou Node.js, Express a Socket.IO.

Pri kolaboratívnom kreslení sa zmena vykonaná jedným používateľom odošle na server a následne sa synchronizuje s ostatnými používateľmi pripojenými do rovnakej miestnosti.


# Materiály

- [Písomná časť diplomovej práce](diplomovka-1.pdf)
- [Prezentácia pokroku](ONLINE%20VEKTOROV%C3%9D%20EDITOR.pptx)
- [Aktuálna verzia aplikácie](vector_editor.zip)
- [Zdrojové kódy aplikácie](DOPLNIŤ_ODKAZ)
- [Spustiteľná online verzia aplikácie](DOPLNIŤ_ODKAZ)
- [Použité knižnice a technológie](DOPLNIŤ_ODKAZ)
- [Materiály k testovaniu](DOPLNIŤ_ODKAZ)


## Aktuálny stav projektu

V súčasnosti je vytvorená **funkčná online verzia kolaboratívneho vektorového editora**. Aplikácia umožňuje viacerým používateľom pripojiť sa do spoločnej miestnosti a pracovať na jednej kresbe v reálnom čase.

Prebehlo pilotné testovanie aj testovanie so žiakmi 9. ročníka. Na základe získanej spätnej väzby pokračuje ďalšia iterácia vývoja, ktorej cieľom je odstrániť identifikované nedostatky a rozšíriť možnosti editora pred finálnym testovaním.

## Súbory v repozitári

- [Písomná časť diplomovej práce](diplomovka-1.pdf)
- [Prezentácia pokroku](ONLINE%20VEKTOROV%C3%9D%20EDITOR.pptx)
- [Aktuálna verzia aplikácie](vector_editor.zip)
