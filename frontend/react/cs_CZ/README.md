# Hierarchický seznam
## Požadované technologie (povinné)
- Typescript
- React
- Apollo Client

## Doporučené technologie (nepovinné)
- Create React App / Next.js, ....
- GraphQL Code Generator
- Router
- UI Framework (jakákoli knihovna) nebo Styled Components
    - React Atlantic (@atlasgroupcz)^
    - Material UI
    - React Bootstrap
    - Ant Design
- Testování
    - Jest
    - React Testing Library

### Samozřejmě můžete použít i jiné technologie, které vám pomohou s vývojem aplikace.
### Později nás může zajímat proč jste (ne)zvolili danou technologii.

## Zadání
Na url https://react-test.atlasconsulting.cz/ běží **GraphQL** server. [Server poskytuje playground](https://react-test.atlasconsulting.cz/).
Vaším úkolem je vytvořit aplikaci, která bude s tímto serverem komunikovat.
Aplikace bude umět vykreslovat hierarchickou strukturu (složka/soubor), při kliknutí na položku
soubor, se zobrazí náhled.
Server obsahuje dvě query.

**1. query** vrací list položek, který bude aplikace využívat pro výpis hierarchického seznamu.
(Položka má v sobě uloženou informaci o tom, zda se má chovat jako složka nebo jako soubor)
Vstupním parametrem je id složky, pokud je parametr prázdný, API vrátí první úroveň (root folder),
výstupem je pak list položek, který patří pod tuto složku.

**2. query** vrací data daného souboru, vstupním parametrem je id.

###Odevzdávat budete **GIT** repozitář se zdrojovými soubory aplikace.

## Bonus
- zavření náhledu
- expand a collapse složek
- cache hierarchické struktury
- cache otevřených souborů
- historie otevřených souborů
- záložky se soubory
    - uživatel může otevírat soubory z hierarchické struktury
    - při otevření souboru se zobrazí náhled tohoto souboru
    - aplikace si ukládá otevřené soubory
    - uživatel má přístup k seznamu otevřených souborů^
    - uživatel může zavírat otevřené soubory ze seznamu
- záložky aplikace
    - uživatel může dynamicky vytvářet a mazat na sobě nezávislé záložky (jako otevřené
      záložky v prohlížeči či plochy v operačním systému)
    - každá nová záložka bude vypadat jako nová aplikace se základním stavem (se
      zavřeným hierarchickým seznamem, bez náhledu a bez seznamu otevřených souborů, řešení musí být v rámci jedné react aplikace )

[Referenční design aplikace](https://wireframe.cc/6JRvnm)


