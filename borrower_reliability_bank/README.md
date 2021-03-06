# **Исследование надежности заемщиков банка.**

***Описание проекта:*** для кредитного отдела банка нужно оценить влияние семейного положения и количества детей клиента на его способность возврата кредита в срок.

***Задачи:***
  - предположить есть ли зависимость между возвратом кредита в срок и:
    - целью кредита;
    - уровнем дохода;
    - семейным положением;
    - наличием детей.
    
***Используемые инструменты:*** python и библиотеки - pandas, pyMystem3.

***Полученные выводы:***
   1. Большинство заемщиков не имеют детей.
   1. Чаще всего не возвращают кредит в срок клиенты, у которых есть дети.
   1. Самый большой процент не возврата у клиентов, у которых семейный статус: Не женат / не замужем. 
   1. Самый высокий процент не возврата у людей с низким уровнем дохода.
   1. Самый высокий процент не возврата кредита в срок, у людей с целью кредита - автомобиль. На втором месте - образование. Самый низкий кредит не возврата у людей, цель которых - покупка жилья.
  
***Описание исследуемых данных:*** датасет, каждая строка которого содержит информацию о клиенте:
  - пол;
  - семейное положение;
  - количество детей;
  - уровень образования;
  - возраст;
  - тип занятости;
  - цель получения кредита;
  - имеется ли задолженность у клиента.
  
  ***Данный проект находится на доработке.*** 
  Изменения, которые планируется внести:
   - выделить сегменты по уровню дохода;
   - для каждого сегмента проверить зависимость между возвратом кредита в срок и всеми признаками:
     - построить распределения данных
     - провести "разведочный" анализ
     - построить матрицу корреляции
     - выявить характерные черты для каждого сегмента с помощью описательной статистики, построения графиков: "ящика с усами", гистограммой.
     - сформулировать гипотезы
     - подтвердить/опровергнуть гипотезы с помощью методов математической статистики
     - сделать вывод.
