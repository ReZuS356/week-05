# KI/DT/22 - 5. tyzden (Seminar 5)

Vypracovane zadania 5. tyzdna z predmetu **Databazove technologie (FPVaI/KI/DT/22)**.
Riesenie je ulozene vo vetve `week-05`.

* **Seminar 5 - Zadanie 1a** - praca so subormi (XLSX, CSV, Parquet), kontrola struktury datasetu a zakladne transformacie, praca s Parquet suborom (schema, metadata, row groups, vyber len potrebnych stlpcov) nad datasetom NYC Green Taxi - januar 2024.
* **Seminar 5 - Zadanie 1b** - validacia dat a spracovanie chyb nad vstupnym suborom `sales_data_dirty.csv` (bezpecne nacitanie, audit datasetu, validacne pravidla, validacny report a oddelenie cistych a problemovych zaznamov).

**Autor:** Vladyslav Nosikov

## Obsah vetvy `week-05`

| Subor | Popis |
| --- | --- |
| `file_handling.ipynb` | Vypracovany notebook - praca so subormi a Parquet (Zadanie 1a) |
| `error_handling.ipynb` | Vypracovany notebook - validacia dat a spracovanie chyb (Zadanie 1b) |
| `west_region_sales.xlsx` | Vystup - predaje z regionu West (XLSX) |
| `it_employees.csv` | Vystup - zamestnanci oddelenia IT |
| `high_salary.csv` | Vystup - zamestnanci s platom nad 80000 |
| `sales_report.parquet` | Vystup - sales_report+(1).csv ulozeny vo formate Parquet |
| `sales_report2.parquet` | Vystup - novy Parquet dataset a jeho rozsirenie o dalsie riadky |
| `partitioned_sales/` | Vystup - Parquet dataset partitionovany podla stlpca Region |
| `sales_data_clean.csv` | Vystup - zaznamy, ktore presli validaciou |
| `sales_data_rejected.csv` | Vystup - zamietnute zaznamy s dovodom zamietnutia |
| `validation_report.csv` | Vystup - pocty chyb podla jednotlivych validacnych pravidiel |
| `employees.csv`, `sales_report.xlsx`, `sales_report+(1).csv` | Vstupne subory pouzite v notebooku `file_handling.ipynb` |
| `green_tripdata_2024-01.parquet` | Prideleny dataset k samostatnym uloham (NYC Green Taxi - januar 2024) |
| `sales_data_dirty.csv` | Vstupny dataset k ulohe 1b |

**Poznamka:** subor `yellow_tripdata_2024-01.parquet` (cca 48 MB) nie je ulozeny v repozitari,
pretoze prekracuje limit pre upload suborov. Notebook si ho v casti 4.1 stiahne sam
(zdroj: `https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_2024-01.parquet`).
