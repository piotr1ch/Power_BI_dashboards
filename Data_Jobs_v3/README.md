# Power BI Dashboard Data Jobs v3

## Opis projektu

Projekt przedstawia dashboard stworzony w Power BI na podstawie danych z 2024 roku dotyczących rynku pracy w obszarze analizy danych.  
Dane pochodzą z kursu [Power BI Course](https://lukebarousse.com/powerbi) autorstwa Luke’a Barousse’a na YouTube.  
Analiza została przeprowadzona w celu nauki i praktycznego opanowania narzędzia Power BI.

W porównaniu do poprzedniej wersji model danych został rozszerzony o nowe źródła:
    
- Populacja krajów (World Bank - SP.POP.TOTL)

- PKB całkowite (current US$) (World Bank - NY.GDP.MKTP.CD)

- PKB per capita (current US$) (World Bank - NY.GDP.PCAP.CD)

Aby dane poprawnie połączyć z istniejącym modelem, konieczne było mapowanie nazw krajów: nazwy w starych danych różniły się od tych pobranych ze strony World Bank.
Część nazw została dopasowana automatycznie (fuzzy match), a brakujące pozycje uzupełniono ręcznie, aby uzyskać spójny model danych.

![Data_Model](/Data_Jobs_v3/Assets/Project_3_Data_Model.png)

## Opis dashboardu



### Page 1 – Data Jobs Dashboard 3.0: Global Job Market Overview

![Page1](/Data_Jobs_v3/Assets/Project_3_Page1.png)

#### KPI:
- Job Count
- Countries in dataset
- Top country (Job Count – nazwa kraju)
- Top country (Job Count – liczba ofert)

#### Tabela top 10 krajów:
Kolumny: Country | Population | GDP | Job Count | Job Density

#### Scatter chart: Population vs Job Count

Dashboard pozwala szybko ocenić wielkość rynku pracy i gęstość ofert względem populacji, a także identyfikować kraje z największą liczbą ofert.


### Page 2 – Economic Factors vs Job Market Performance

![Page2](/Data_Jobs_v3/Assets/Project_3_Page2.png)

#### Scatter charts:
- GDP per Capita vs Job Density
- GDP per Capita vs Job Count
- Slicer: Population tier (0–10M, 10–20M, 20–100M, 100M+)

Strona ta pokazuje zależności między PKB (total i per capita) a rynkiem ofert pracy, umożliwiając analizę ekonomiczną w kontekście liczby i gęstości ofert w różnych krajach.

## Zakres umiejętności

- Estetyczne i funkcjonalne projektowanie dashboardów
- Czyszczenie i przygotowanie danych w Power Query
- Mapowanie i scalanie danych z różnych źródeł (World Bank + kursowe dane)
- Modelowanie danych (star schema)
- Podstawy języka DAX (KPI i miary)
- Praca z Visual Studio Code
- Wykorzystanie Git i GitHub do wersjonowania projektów

## Podsumowanie

Rozszerzenie modelu o dane makroekonomiczne i mapowanie krajów pozwoliło dodatkowo analizować zależności między wielkością rynku a czynnikami gospodarczymi, co zwiększa wartość analityczną dashboardu.