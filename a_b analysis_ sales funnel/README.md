# **Исследование для интернет-магазина**



***Описание проекта***:
 был проведен эксперимент: пользователей интернет-магазина поделили на три группы (в двух группах оставили старый шрифт, а в третьей - изменили). Нужно оценить влияние  шрифта на количество клиентов, "проходящих" по воронке продаж. 

 Данное исследование является завершенным, доработки не предполагаются.

***Задачи***:
  - установить шаги в воронке продаж;
  - изучить воронку продаж;
  - проверить критерий успешности А/А теста;
  - установить в какой группе А или В шрифт лучше.

***Используемые инструменты:***
   - python, библиотеки - pandas, numpy, matplotlib, seaborn, plotly, scipy.


***Выводы:***
  1. Предполагаемые шаги в воронке:
    А: MainScreenAppear - главная страница 
    B: OffersScreenAppear - переход в каталог
    C: CartScreenAppear - корзина
    D: PaymentScreenSuccessful - оплата
    F: Tutorial - руководство
    
События происходят в следующем порядке: A ---> B ---> C ---> D, или, A ---> F
  1. Все шаги выстраиваются в привычном для воронки виде. Пользователям не приходится совершать не логичных действий, чтобы добраться до шага D: PaymentScreenSuccessful(оплата).
  1. 47% пользователей (хоть раз совершивших действие)  доходят до шага D: PaymentScreenSuccessful(оплата) от общего числа пользователей.
  1. По воронке последовательности действий 6% пользователей(от числа пользователей на предыдущем шаге) и 26% от общего числа пользователей "доходят" до шага D: PaymentScreenSuccessful(оплата) .
  1. Существуют иные пути, отличные от предполагаемых шагов, чтобы добраться до шага D: PaymentScreenSuccessful(оплата).
  1. Критерии успешности А/А теста выполнены:
     - количество пользователей в группах различается не более, чем на 1%;
     - различие ключевых метрик (доли пользователей хоть раз совершивших действие от общего числа уникальных пользователей) не имеет статист. значимости.
     Разбиение на группы работает корректно.
  1. Значимых различий между двух групп со старым и новым шрифтом выявлено не было. 


***Исследуемые данные:*** файл с логами. Каждая строка которого содержит информацию об одном действий пользователя: идентификатор, дату и время, название события(действия), номер эксперимента.

Также стоит отметить, что в работе используются стат.критерии на одних  данных сначала без использования поправки на множественность тестов, а затем эти критерии с использованием - это сделано умышленно, чтобы оценить и понять значимость поправки множественности тестов (в частности, в работе использована поправка Бонферрони).

*NOTEBOOK.ipynb лучше смотреть через [https://nbviewer.jupyter.org/]: чтобы была возможность отследить интерактивность графиков, ссылок.*
