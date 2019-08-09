# Python

### Obecný účel zadání

Chceme získat rozšiřitelný dataset textových dat (z novin/článků/knih/časopisů nebo čehokoliv jiného) pro následné vytvoření analýzy textových dat v češtině.

### Zadání

1. Napište scraper pro stahování dat nejnovějších článků z online serverů. Můžete využít servery jako [idnes.cz](https://www.idnes.cz/), [novinky.cz](https://www.novinky.cz/), [sport.cz](https://www.sport.cz/), případně cokoliv jiného (vyberte si alespoň 1). Scraper bude vycházet ze stránky seznamu nejnovějších článků a postupně se "proklikávat" do detailu jednotlivých článků, případně seznamu komentářů. Skript bude mít alespoň 1 vstupní parametr na omezení stahování (např. cílový počet stažených článků, podle data apod.). Dále bude ošetřený na nejčastější runtime chyby (např. detail článku vrátí chybu 404, vypadne na chvíli spojení se serverem, nepodaří se navázání HTTPS spojení apod.)
2. Ze stažených článků se pokuste vyextrahovat maximum dostupných relevantních informací (nadpis, datum zveřejnění, autor, vlastní text, komentáře, počet zhlédnutí, ...) a vytvořte z nich strukturovaný objekt, který uložíte do NoSQL databáze.
3. Nad uloženými daty napište jednoduché API (např. flask), které dokáže vracet (vyberte si alespoň 2):
   - N nejnovějších článků
   - N nejkomentovanějších článků
   - N nejpoužívanějších slov
   - N nejdelších slov

Příklad struktury uloženého článku:

```python
item = {
    'link': 'https://www.idnes.cz/olomouc/zpravy/olomouc-rekonstrukce-ulice-8-kvetna-zuzeni-chodniku-opozice-barva-vandalstvi-cisteni.A190809_494437_olomouc-zpravy_stk',
    'header': 'Opozice vyznačila křídou chystané zúžení chodníku, rozzlobila primátora',
    'category': 'Olomoucký kraj',
    'author': 'Ondřej Mazoch',
    'published_at': '2019-08-09',
    'paragraphs': [
        'Dost svérázně dali najevo nesouhlas s chystanými ...',
        'Akci, která má podle organizátorů ukázat chybnou ...',
        '„Ukázali jsme občanům, jak by situace vypadala ...',
    ],
}
```

Zadání je záměrně neurčité a je na vás, jak si s ním poradíte.

### Technologie

- Povinné
  - Python 3.x
  - knihovna [Scrapy](https://scrapy.org/)
  - NoSQL databáze [MongoDB](https://www.mongodb.com/)
  - knihovna [Flask](https://flask.palletsprojects.com/en/1.1.x/)
- Doporučené
  - Docker
  - Pytest
  - cokoliv :)

### Odevzdání

- Odkaz na veřejný git repozitář, např. [GitHub](https://github.com/), [GitLab](https://gitlab.com/)
- Obsah:
  - skript pro stahování dat
  - skript s API
  - návod ke spuštění


<details><summary><b>Teaser</b></summary>
<p>

lambda, list, tuples, open(), zip()

</p>
</details>
