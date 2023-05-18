# Тестовое задание для компании Улыбка Радуги (вакансия аналитик данных)



***СТАТУС:*** **Завершён**


## Цели проекта:

Необходимо выполнить тестовое задание, включающее в себя составление пяти SQL запросов на основе имеющихся данных. Решение задачи по оценке результатов А/Б теста. Очистка набора данных от выбросов и аномалий.

## Задачи:

### SQL 1:

Даны 4 колонки: Магазин, Город, Код товара, Товарное направление

Условие:
Необходимо получить все возможные варианты магазин-товар (без использования таблицы SALES)

#### Результат выполнения задания SQL 1:

<img src="https://i.imgur.com/NacBKXS.png" alt="SQL1"/>

### SQL 2:

Дано 5 колонок: Магазин, Город, Адресс, Сумма в шт, Сумма в руб

Условие:
Необходимо получить все возможные варианты магазин-товар (без использования таблицы SALES)

#### Результат выполнения задания SQL 2:

<img src="https://i.imgur.com/6mVHGYg.png" alt="SQL2"/>

### SQL 3:

Дано 3 колонки: Дата, Город, Доля в суммарных продажах в руб на дату

Условие:
Выборка только по товарам направления ЧИСТОТА

#### Результат выполнения задания SQL 3:

<img src="https://i.imgur.com/9vs5IQv.png" alt="SQL3"/>

### SQL 4:

Дано 3 колонки: Дата, Магазин, Товар

Условие:
Информация о топ-3 товарах по продажам в штуках в каждом магазине в каждую дату

#### Результат выполнения задания SQL 4:

<img src="https://i.imgur.com/n5WKzWL.png" alt="SQL4"/>

### SQL 5:

Дано 4 колонки: Дата, Магазин, Товарное направление, Сумма в руб за предыдущую дату

Условие:
Только магазины СПб

#### Результат выполнения задания SQL 5:

<img src="https://i.imgur.com/fyKpfXO.png" alt="SQL5"/>

### Задание по оценке результатов А/Б теста:

Дано:

Был произведен отбор покупателей (17 744), у которых скоро День рождения, для отправки им поздравительной смс-рассылки и оповещения о персональной скидке.
Полученную выборку случайным образом разделили на целевую (получили рассылку) и контрольную группы в соотношении 75% к 25%. 
Акция длилась 3 дня.
Ниже в таблице предоставлены данные о количестве откликнувшихся на предложение покупателей в каждой из групп за период проведения акции. Также известно, что коэффициент доставляемости сообщений по результатам этой рассылки составил всего 2/3 от общего объёма рассылки.

Требуется:

Посчитать количество дополнительно привлечённых благодаря рассылке покупателей. Формулы сохранить в файле.

#### Результат выполнения задания:

<img src="https://i.imgur.com/3oORjch.png" alt="Excel"/>

Полное решение с формулами доступно в Excel файле в этом репозитории.

### Задание по очистке данных от выбросов:

Дано:

На листе "Данные для очистки" приведены подневные продажи в штуках одного магазина за период январь 2020 - май 2022. В динамике продаж наблюдаются как устойчивые закономерности, так и аномальные значения. 

Требуется:

Найти выбросы в данных, осуществить их замену с учётом обнаруженных закономерностей. 
Формулы сохранить в файле. В случае использования для решения языков программирования R/Python приложить скрипт со всеми этапами обработки данных.

#### Результат выполнения задания:

Визуализация первичных данных:

<img src="https://i.imgur.com/FoBNZkd.png" alt="vid1"/>

Визуализация данных после обработки выбросов:

<img src="https://i.imgur.com/nEl9yj9.png" alt="vid2"/>

Обработка выбросов, в данном ТЗ, показалась работадателю некачественной. Проанализировав недочеты, было принято решение обратиться за помощью к нейронной сети, которая определила все выбросы, опираясь на алгоритм поиска выбросов LSTM Autoencoder.

Вот ее результат:

<img src="https://i.imgur.com/Nz8Kv0n.png" alt="vid3"/>

Вид датасета после замены всех выбросов с учетом замеченых закономерностей:

<img src="https://i.imgur.com/61aPxrv.png" alt="vid4"/>

---

<img src="https://i.imgur.com/CxBDSVg.png" alt="vid5"/>

Код c пояснениями доступен в рамках данного репозитория.

## Инструменты проекта

- Python
- Pandas
- Sklearn
- Matplotlib.pyplot
- Keras
- SQLite3
