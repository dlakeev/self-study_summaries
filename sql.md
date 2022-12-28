# With as
Используется для того, чтобы "запаковать" запрос.
### Пример
```sql
WITH AS name_ as (
    SELECT *
    from table_name
)

SELECT *
from name_
```
___
# Пересечение множеств
## Join

<p align="center">
  <img src="https://www.postgresqltutorial.com/wp-content/uploads/2018/12/PostgreSQL-Joins.png">
</p>

___
## Другие
* **_UNION_** по сути добавляет результаты второго запроса к результатам первого (хотя никакой порядок возвращаемых строк при этом не гарантируется). Более того, эта операция убирает дублирующиеся строки из результата так же, как это делает DISTINCT, если только не указано UNION ALL.

* **_INTERSECT_** возвращает все строки, содержащиеся в результате и первого, и второго запроса. Дублирующиеся строки отфильтровываются, если не указано ALL.

* **_EXCEPT_** возвращает все строки, которые есть в результате первого запроса, но отсутствуют в результате второго. (Иногда это называют разницей двух запросов.) И здесь дублирующиеся строки отфильтровываются, если не указано ALL.
___

# Оконные функции