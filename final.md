# Projekt końcowy

## Wprowadzenie

W końcowym projekcie Twoim zadaniem będzie wykorzystanie **umiejętności** nabytych na tych zajęciach do *eksploracyjnej analizy danych* dotyczącej rzeczywistego zestawu danych (lub zestawów danych).

Będziesz pracować w małej grupie (2-3 osoby), ale gorąco zachęcam do kontaktu, aby uzyskać informacje zwrotne na temat swoich pomysłów.

## Ocenianie i rezultaty

Końcowym rezultatem (tym, co oddasz) będzie link do REPO na GitHubie, w którym Twój zespół umieści wszystkie pliki projektu: 

- notatnik Jupyter z następującymi sekcjami (patrz tabela poniżej); każda sekcja jest warta określoną liczbę punktów, sumując do 17; **końcowa propozycja projektu** jest również warta 1 punkt.
- dane (np. pliki CSV).
- dodatkowe pliki, mile widziane opublikowane estetycznie raporty EDA w formacie Markdown (MD, PDF itp.)




| Sekcja | Punkty | Opis | Przykład 1 | Przykład 2 |
| --------------- | ---- | ---------- | -------- | ------- |
| Wprowadzenie | 2 | Na jaki zbiór danych patrzysz? Gdzie/jak został utworzony? Jakie pytania będą zadawane? | Zbiór danych o tym, której konstrukcji ludzie używają w [alternacji celownika](http://www.glottopedia.org/index.php/Dative_alternation): czy używają NP („Dała mężczyźnie pudełko”) czy PP („Dała pudełko mężczyźnie”). Zapytam, które cechy przewidują użycie jednej konstrukcji w porównaniu z drugą. | |
| Wizualizacje | 4 | 2-3 wykresy przedstawiające określone wzorce lub cechy, które chcesz podkreślić. Każdej wizualizacji powinien towarzyszyć krótki (1-2 zdania) opis tego, co według Ciebie pokazuje. | Boxplot pokazujący **długość** argumentu *tematu*, gdy odbiorca jest realizowany jako fraza rzeczownikowa vs. fraza przyimkowa. Wykres słupkowy pokazujący proporcję realizacji **NP** w zależności od animacji odbiorcy. | | 
| Analizy | 4| 2-3 analizy omówione w klasie (np. regresja liniowa, itp.), aby odnieść się do pytania. Każdej analizie powinna towarzyszyć krótka (1-3 zdania) *interpretacja*. Powinna również zawierać **ocenę** modelu, np. $R^2$, AIC, itp. | Regresja logistyczna przewidująca **realizację** (NP vs. PP) z Animacji i Długości. Porównaj AIC tego modelu z modelem pomijającym każdą zmienną po kolei. | |
| Ograniczenia i kwestie etyczne| 3 | Omów wszelkie ograniczenia swojego podejścia, a także potencjalne kwestie etyczne (jeśli dotyczy). | Zmienne mogą być ze sobą powiązane; łącznie tylko 4 zmienne predykcyjne. | |
| Wnioski | 1 | Wyciągnięcie wniosków na temat zbioru danych i postawionych pytań. | Realizacja NP jest bardziej prawdopodobna w przypadku *dłuższych tematów*.


### Przykładowe zbiory danych

Istnieją dwa krytyczne wymagania dotyczące zestawu danych:

1. Po pierwsze, powinien on dotyczyć **danych z zakresu nauk społecznych**. Jeśli nie masz pewności, czy dany zestaw danych się kwalifikuje, możesz nas zapytać.  
2. Po drugie, powinien zawierać co najmniej **3 zmienne** (ale najlepiej więcej). Nie chcemy, abyś analizował tylko jedną zmienną, ani jak jedna zmienna odnosi się do jednej innej zmiennej. Idealnie byłoby, gdybyś wziął pod uwagę związek wielu zmiennych (np. w **regresji wielokrotnej**). 

Mając to na uwadze, oto kilka pomysłów na **odpowiednie zestawy danych**. Możesz skorzystać z jednego z nich (i zadać pytania, które uważasz za interesujące), ale możesz też znaleźć własny; te zestawy danych zostały **zweryfikowane** nieco bardziej.

| Zbiór danych | Dziedzina nauk społecznych | Opis | Dostęp |
| ------ | ---- | ---------- | ------- |
| World Bank Open Data | Economics / Global Development | Contains time series data for **many domains**, such as agricultural development, rural poverty, carbon emissions, and much, much more. | [Link to Data Bank](https://data.worldbank.org/); can browse by "indicator"; may require merging datasets for more information. |
| [World Happiness Report](https://www.kaggle.com/datasets/ajaypalsinghlo/world-happiness-report-2021) | Economics / Global Development | Dataset about global happiness scores; might need to be merged with other datasets to ask useful questions. | [Kaggle](https://www.kaggle.com/datasets/ajaypalsinghlo/world-happiness-report-2021)|
| World Energy Consumption | Contains time series data about consumption of **energy** and **electricity**. | [Link on Kaggle](https://www.kaggle.com/datasets/pralabhpoudel/world-energy-consumption) |
| SCARFS (Spontaneous, controlled, acts of reference between friends and strangers) | Linguistics/Communication | Data about friends and strangers playing the game **Taboo**, which clues they gave, and whether a trial was wason. | [GitHub Link](https://github.com/seantrott/scarfs) |
| [California Housing Prices](https://www.kaggle.com/datasets/camnugent/california-housing-prices) | Economics | Information about the median house value for different districts in California. | [Link on Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices). |
| [Student alcohol consumption](https://www.kaggle.com/datasets/uciml/student-alcohol-consumption?select=student-por.csv) | Public Health | Information about student behavior, including alcohol consumption and more. |  [Link on Kaggle](https://www.kaggle.com/datasets/uciml/student-alcohol-consumption?select=student-por.csv). |
| [Dative Alternation](https://rdrr.io/cran/languageR/man/dative.html) | Linguistics | Dataset about which construction people use in the dative alternation: do they use NP ("She gave the man the box") or PP ("She gave the box to the man"). | Online, or ask Professor Trott for `.csv` file |


### Trudność projektu

Należy pamiętać, że weźmiemy również pod uwagę **trudność** związaną z projektem, zwłaszcza na etapie **danych** (np. czyszczenie danych, łączenie wielu zestawów danych). 

Znalezienie i połączenie wielu zestawów danych nie jest *konieczne* - tzn. można uzyskać pełne punkty bez tego - ale jeśli pomyślnie wyczyścisz i połączysz wiele zestawów danych, może to „zrównoważyć” niższe wyniki w innej sekcji (np. **Wizualizacja**); czyli możesz myśleć o tym jako o rodzaju nieoficjalnego dodatkowego kredytu.

Oto kilka przykładów rzeczy, które, choć nie są konieczne, uczyniłyby twój projekt trudniejszym, a tym samym bardziej imponującym:

- **Łączenie** wielu zestawów danych, które znalazłeś, aby wykorzystać powiązanie danych.  
- **Porównanie** wielu modeli statystycznych przy użyciu metod *wyboru modelu*, które omawialiśmy na zajęciach. 

