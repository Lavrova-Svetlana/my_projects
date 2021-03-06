# **Приоритизация гипотез. Анализ результатов А/В теста**

Целью данной работы являлось:
  - раставление приоритетов гипотез с помощью использования фреймворков: ISE SCORE и RICE SCORE и сравнение полученных результатов;
  - принятие решения об остановке А\В теста либо его продолжение на основании анализа его результатов.

В ходе работы были использованы инструменты: python, библиотеки - pandas, matplotlib, scipy.

Изначально было получено три датасета:
  - о гипотезах. Каждая строка датасета соответствует одной гипотезе и содержит информацию: название, оценку, выставленую по 10-бальной шкале: охват пользователей, влияние на пользователей, уверенность в гипотезе, затраты ресурсов на проверку гипотезы;
  - о заказах в группах А/В теста. Каждая строка соответствует одному заказу и содержит информацию: идентификатор заказа; идентификатор пользователя, совершившего заказ; дату, когда был совершен заказ; сумму выручки от заказа; группу A/B-теста, в которую попал заказ;
  - о пользователях в группах А/В теста. Содержит информацию о количестве пользователей в указанной группе в указанную дату.

Структура проекта:
  - Изучение общей информации о полученных данных в файле;
  - Предобработка данных;
  - Приоритизация гипотез:
    - с использованием ICE SCORE;
    - с использованием RICE SCORE;
    - вывод.
  - Анализ А/В теста:
    - построение графика кумулятивной выручки по группам А/В теста;
    - построение графика кумулятивного среднего чека по группам А/В теста; 
    - построение графика относительного изменения кумулятивного среднего чека гр.В к гр.А; 
    - построение графика кумулятивной конверсии по группам А/В теста;
    - построение графика относительного изменения кумулятивной конверсии гр.В к гр.А;
    - построение точечного графика количества заказов по пользователям, стоимостей заказов;
    - определение выбросов в распределениях количества заказов на пользователя, в распределении стоимости заказов;
    - выдвижение гипотезы и проверка различий в конверсии, в среднем чеке заказа между группами по "сырым" данным;
    - выдвижение гипотезы и проверка различий в конверсии, в среднем чеке заказа между группами по "очищенным" данным;
  - Общий вывод.
