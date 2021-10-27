# Laboratorium 4 - Materiał, Notatki

## SQL CREATE TABLE
Tabelę w SQL tworzymy poleceniem `CREATE TABLE`.

## SQL INSERT INTO
Aby uzupełnić tabelę danymi, używamy polecenia `INSERT INTO`.

## SQL JOIN (+ wariacje)
`JOIN` pozwala na łączenie kolumn z różnych tabeli.

### INNER JOIN
Podstawowe łączenie tabeli - po prostu dokładamy kolejne kolumny. Żadna z kolumn nie może zawierać wartości NULL.

### OUTER JOIN
 - `LEFT OUTER JOIN` - zwraca wszystkie rekordy z lewej tablicy oraz te z prawej, które spełniają warunek złączenia. Brakujące elementy uzupełnione będą wartością NULL.
 - `RIGHT OUTER JOIN` - zwraca wszystkie rekordy z prawej tablicy oraz te z lewej, które spełniają warunek złączenia. Brakujące elementy uzupełnione będą wartością NULL.
 - `FULL OUTER JOIN` - zwraca wiersze dla których warunek jest spełniony, wiersze bez odpowiedników w łączonych tabelach.

## PODZAPYTANIA (Subqueries)
Możemy używać zagnieżdżonych poleceń `SELECT`, aby uzyskać bardziej złożone zapytania. Dobrą zasadą jest umieszczanie jak "najmniejszych" zapytań jak najgłębiej (najbardziej zagnieżdżone). Podzapytania mogą być używane w:
 - `SELECT`
 - `UPDATE`
 - `DELETE`
 - funkcjach agregujących
 - podczas definiowania tabel tymczasowych

## EXPLAIN
Klauzula `EXPLAIN` może służyć do przeanalizowania zapytań pod względem zarówno danych, jakie zwracają, ale i wydajności.

## Funkcje agregujące
Mogą one być wywołane na zestawie wierszy i zwracają jeden wiersz. Dalej standardowe funkcje agregujące.

### AVG()
Zwraca średnią wartość.

### COUNT()
Zwraca ilość.

### MAX()
Zwraca wartość maksymalną.

### MIN()
Zwraca wartość minimalną.

### SUM()
Zwraca sumę.

## GROUP BY
Klauzula ta dzieli zapytanie na grupy. Pojawia się od razu po `FROM` lub `WHERE`. Często stosowana w połączeniu z `SUM()` lub innymi funkcjami agregującymi.

## HAVING
Filtruje grupy (zwrócone z `GROUP BY`), które nie spełniają podanego warunku.
