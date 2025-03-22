# Проект 2. Анализ вакансий из HeadHunter


## Оглавление
[1. Описание проекта](#описание-проекта)  
[2. Какой кейс решаем?](#какой-кейс-решаем)   
[3. Требования к оформлению ноутбука-решения](#требования-к-оформлению-ноутбука-решения)  
[4. Результаты исследования](#результаты)    
[5. Выводы](#выводы)   
[6. Использованные инструменты и библиотеки](#использованные-инструменты-и-библиотеки)    


## Описание проекта
Работа происходит с базой данных соискателей с сайта HeadHunter. 
В данном проекте осуществляется применение sql-запросов в Python и их обработка

⭐ Я устроился на работу в кадровое агентство, которое подбирает вакансии для IT-специалистов. Мой первый проект — создание модели машинного обучения, которая будет рекомендовать вакансии клиентам агентства, претендующим на позицию Data Scientist. Сначала мне необходимо понять, что из себя представляют данные и насколько они соответствуют целям проекта. И провести  Data Understanding (анализ данных).      

[к оглавлению](#Оглавление)

## Какой кейс решаем?

Мой проект включает в себя несколько этапов:
1. Знакомство с данными;
2. Предварительный анализ данных;
3. Детальный анализ вакансий;
4. Анализ работодателей;
5. Предметный анализ.

[к оглавлению](#Оглавление)

## Требования к оформлению ноутбука-решения

* Решение оформляется только в Jupyter Notebook.
* Решение оформляется в соответствии с ноутбуком-шаблоном.
* Каждое задание выполняется в отдельной ячейке, выделенной под задание (в шаблоне они помечены как ваш код здесь). Не следует создавать множество ячеек для решения задачи — это создаёт неудобства при проверке.
* Код для каждого задания оформляется в одной-двух jupyter-ячейках (не стоит создавать множество ячеек для решения задачи, это усложняет проверку).
* Текст SQL-запросов и код на Python должны быть читаемыми. Не забывайте про отступы в SQL-коде.
* Выводы по каждому этапу оформляются в формате Markdown в отдельной ячейке (в шаблоне они помечены как ваши выводы здесь).
* Выводы можно дополнительно проиллюстрировать с помощью графиков. Они оформляются в соответствии с теми правилами, которые мы приводили в модуле по визуализации данных.
* Не забудьте удалить ячейку с данными соединения перед фиксацией работы в GitHub.

[к оглавлению](#Оглавление)

## Результаты исследования:

- Больше всего вакансий в Москве(5333) и Санкт-Петербурге(2851). 
- Средние значения нижней и верхней зарплатной вилки ~71065 и ~110537. 
- Большинство вакансий у нас расчитаны на полный рабочий день - с полной занятостью, для оставшихся численность вакансий резко падает.  
- Среди регионов, в которых нет вакансий, в котором наибольшее количество работодателей является Россия(410). 
- Самой большой компанией является Яндекс, она публикует вакансии в 181 регионе. Oбщее количество вакансий компании Яндекс для городов-миллионников 485, самым большим среди вакансий является Москва- 54.
- Количество работодателей у которых не указана сфера деятельности - 8419. 
- У 3553 вакансий работодателей указана "Разработка программного обеспечения". 
- Мы также определили, что кандидат с опытом работы от 3 до 6 лет может претендовать на заработную плату в размере ~243115 руб. Количество вакансий уменьшается по мере роста опыта.
- В наших данных есть 1771 которые имеют отношения к данным. Для начинающих дата-сайентистов доступно только 51 из них, что является довольно небольшим количеством. Однако, если использовать SQL или Postgres в качестве ключевого навыка, то количество вакансий почти увеличится в 4 раза. Стоит учесть, что включение этих навыков может привести к тому, что поиск уже не будет ограничиваться только начинающими специалистами. Количество вакансий, где требуется использование языка Python, составляет 351. В среднем для вакансий, связанных с Data Science, требуется 6,41 ключевых навыков. 

## Выводы:

Профессия дата сайентиста востребована. Большой строс на Data Science сосредоточен в Москве и Санкт-Петербурге. На hh.ru сейчас примерно 480 вакансий по запросу Data Scientist. При этом больше 217 из них приходятся на столицу, 64 — на Питер, немногим больше 20 — на пару городов-миллиоников, а дальше числа стремительно уменьшаются. Но переезжать не обязательно. Можно работать на удаленке, несмотря на то, что преждложений по удаленной работе меньше в 3 раза, чем работы в офисе, средняя з/п выше примерно на 20%.
Подробнее с выводом можно ознакомится в [ноутбуке](https://github.com/.ipynb) - глава "Дополнительные исследования"

[к оглавлению](#Оглавление)

## Использованные инструменты и библиотеки:

* pandas
* psycopg2
  
## Автор
Зарубин Алексей

[к оглавлению](#Оглавление)
