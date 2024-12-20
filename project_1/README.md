<center> <img src = https://raw.githubusercontent.com/AndreyRysistov/DatasetsForPandas/main/hh%20label.jpg alt="drawing" style="width:400px;">

# Data Science проект: Анализ резюме из HeadHunter
___
## Оглавление
- [Data Science проект: Анализ резюме из HeadHunter](#data-science-проект-анализ-резюме-из-headhunter)
  - [Оглавление](#оглавление)
    - [1. Описание проекта](#1-описание-проекта)
    - [2. Какой кейс решаем](#2-какой-кейс-решаем)
    - [3. Этапы работы над проектом](#3-этапы-работы-над-проектом)
    - [4. Краткая информация о данных](#4-краткая-информация-о-данных)
    - [5. Комментарии по оформлению и визуализации](#5-комментарии-по-оформлению-и-визуализации)
___

### 1. Описание проекта
В нашем распоряжении база резюме, выгруженная с сайта поиска вакансий [hh.ru](https://hh.ru).

Файлы с исходными данными можно скачать [здесь](https://drive.google.com/drive/folders/1Wvx8ewiY1Akng4aOa6v42SWPR2QtGU7f?usp=drive_link).

### 2. Какой кейс решаем

**Проблематика:** часть соискателей не указывает желаемую заработную плату, когда составляет своё резюме.

Это является помехой для рекомендательной системы HeadHunter, которая подбирает соискателям список наиболее подходящих вакансий, а работодателям — список наиболее подходящих специалистов.

⭐ Компания *HeadHunter* хочет построить модель, которая бы автоматически определяла примерный уровень заработной платы, подходящей пользователю, исходя из информации, которую он указал о себе. Но прежде чем построить модель, данные необходимо преобразовать, исследовать и очистить. В этом и состоит задача этого проекта.

:arrow_up: [к оглавлению](#оглавление)

### 3. Этапы работы над проектом
1. Базовый анализ структуры данных
2. Преобразование данных
3. Разведывательный анализ (EDA)
4. Очистка данных

### 4. Краткая информация о данных
Исходный датасет (выгрузка из hh.ru анкет кандидатов) представляет собой таблицу с 12 колонками-параметрами и 44744 строками.

**Колонки:**
+ Пол, возраст
+ ЗП
+ Ищет работу на должность
+ Город, переезд, командировки
+ Занятость
+ График
+ Опыт работы
+ Последнее/нынешнее место работы
+ Последняя/нынешняя должность
+ Образование и ВУЗ
+ Обновление резюме
+ Авто

:arrow_up: [к оглавлению](#оглавление)

### 5. Комментарии по оформлению и визуализации
+ Проект оформлен в виде ноутбука [Project-1. HH.ipynb](https://github.com/olegrasskazovpro/sf_data_science/blob/main/project_1/Project-1.%20HH.ipynb) со всеми комментариями, выводами, кодом и диаграммами.

+ За внешний вид диаграмм отвечает переменная `plot_format` в начале ноутбука. Она установлена в значение 'jpg', т.к. использовались интерактивные визуализации Ploty, которые GitHub не умеет отображать. Чтобы увидеть интерактивные диаграммы, достаточно запустить ноутбук на локальной машине, присвоив `plot_format = ''`

![Зависимость медианной ЗП от возраста и образования](images/med_zp_vozrast_edu.jpeg)