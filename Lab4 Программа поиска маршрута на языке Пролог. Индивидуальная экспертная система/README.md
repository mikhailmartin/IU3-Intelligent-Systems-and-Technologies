# Лабораторная работа №4 на тему «Программы поиска маршрута на языке логического программирования Пролог. Индивидуальная экспертная система»

## Задание 1
Задание представлено в виде квадратной матрицы размером 6х6. Она задаёт лабиринт из пещер и проходов между ними.

| номер пещеры | 1   | 2   | 3   | 4   | 5   | 6   |
|:------------:|-----|-----|-----|-----|-----|-----|
|      1       | 0   | 0   | 1   | 0   | 0   | 0   |
|      2       | 0   | 0   | 0   | 0   | 1   | 1   |
|      3       | 1   | 0   | 0   | 1   | 0   | 0   |
|      4       | 0   | 0   | 1   | 0   | 1   | 0   |
|      5       | 0   | 1   | 0   | 1   | 0   | 0   |
|      6       | 0   | 1   | 0   | 0   | 0   | 0   |

1 - проход между пещерами есть; 0 - прохода нет. В каждой пещере есть одно содержимое. Пещеры именованы содержимым.
Необходимом написать программу нахождения пути, ведущего от входа к выходу через клад и не через пещеры с опасностями.

## Задание 2
Разработать и отладить на языке логического программирования Visuаl Prolog экспертную систему, позволяющую по
результатам ответа экспертной системе определять, в какой степени данный студент известен отвечающему на вопросы.
Экспертная система должна использовать динамическую базу данных и функционировать следующим образом:

1. После запуска программы должно появиться сообщение «Вы интересуетесь сведениями о студенте <имя и фамилия> кафедры
ИУ-3 «Информационные системы и телекоммуникации» группы <номер группы>. Отвечайте «да» или «нет» на задаваемые вам
вопросы (y/n)».
2. Далее программа по порядку задает пользователю вопросы. Например:
   * Близкие родственники: отец: фамилия: Иванов?
   * Близкие родственники: отец: имя: Иван?
   * Близкие родственники: отец: отчество: Иванов?
3. Пользователь отвечает «да» или «нет» путём ввода символов «y» или «n» с клавиатуры.
4. После ответа на все заданные вопросы печатается сообщение: «Вы ответили правильно на m вопросов из n возможных», где
n и m – соответственно общее количество вопросов и количество правильных ответов пользователя.
5. Далее выводится список вопросов, на которые пользователь ответил правильно с указанием ответов пользователя. А затем,
список вопросов, на которые пользователь ответил неправильно также с указанием ответов пользователя.
6. И, наконец, выдается сообщение: «C уверенностью <коэффициент уверенности>% студент <имя и фамилия студента> группы
<номер группы> кафедры «Информационные системы и телекоммуникации» удовлетворяет вашим ответам».
7. Коэффициент уверенности вычисляется как отношение m/n.
