# Java homework assignment

### Level 1 (junior)

**Zadání:**

Business chce na titulní straně aplikace CODEXIS ukazovat nejpopulárnější dokumenty za poslední týden - tj. ty, jejichž otevíranost u uživatelů byla největší. Identifikátor dokumentu i uživatele je UUID.

Navrhněte a napište microservice, která bude tuto funkcionalitu zajišťovat - sbírat data o otevíranosti dokumentů (buďto navrhněte API, nebo předpokládejte, že tyto data chodí např. do nějaké event queue), dále bude appka poskytovat výstup dle zadání. Funkcionalitu microservice demonstrujte integračním testem, které si potřebné prostředí (databázi, atd.) vytvoří pomocí Test Containers - https://www.testcontainers.org/).
Odevzdání:

Projekt odevzdejte jako gitové repository (např. na githubu).

**Hodnocení:**

Jsou hodnocena tato kritéria:
- čistota kódu
- výpočet nejpopulárnějších dokumentů
- efektivita dotazů


### Level 2 (intermediate)

**Zadání:**

Business chce na titulní straně aplikace CODEXIS ukazovat “trending” dokumenty za poslední týden - tj. ty, jejichž otevíranost u uživatelů není zanedbatelná a má rostoucí a zrychlující tendenci. Identifikátor dokumentu i uživatele je UUID.

Navrhněte a napište microservice, která bude tuto funkcionalitu zajišťovat - sbírat data o otevíranosti dokumentů (buďto navrhněte API, nebo předpokládejte, že tyto data chodí např. do nějaké event queue), dále bude appka poskytovat výstup dle zadání. Funkcionalitu microservice demonstrujte integračním testem, které si potřebné prostředí (databázi, atd.) vytvoří pomocí Test Containers - https://www.testcontainers.org/).
Odevzdání:

Projekt odevzdejte jako gitové repository (např. na githubu).

**Hodnocení:**

Jsou hodnocena tato kritéria:
- čistota kódu
- elegance výpočtu trending dokumentů
- efektivita dotazů
- efektivita zpětných pohledů v čase na trending dokumenty v jednotlivých týdnech




### Level 3 (senior)

**Zadání:**

Business chce na titulní straně aplikace ukazovat “trending” dokumenty za poslední týden - tj. ty, jejichž otevíranost u uživatelů není zanedbatelná a má rostoucí tendenci. Analytické oddělení chce mít možnost pohledu na tyto “trending” dokumenty v libovolném historickém období.


Navrhněte a napište microservice, která bude tuto funkcionalitu zajišťovat - sbírat data o otevíranosti dokumentů (API si navrhněte) a poskytovat výstup dle zadání. Funkcionalitu microservice demonstrujte integračním testem, které si potřebné prostředí (databázi, atd.) vytvoří pomocí Test Containers - https://www.testcontainers.org/).  Tip - použijte nějakou event queue.

**Odevzdání:**

Projekt odevzdejte jako gitové repository (např. na githubu).

**Hodnocení:**

Jsou hodnocena tato kritéria:
- čistota kódu
- elegance výpočtu trending dokumentů
- efektivita dotazů
- efektivita zpětných pohledů v čase na trending dokumenty v jednotlivých týdnech






