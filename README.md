# Вступительное задание

Привет! Если ты читаешь этот текст — ты на полпути к поступлению на курс front-end middle.
Мы очень хотим, чтобы курс приносил студентам максимальную пользу, поэтому просим тебя выполнить небольшое
вступительное задание. Это позволит нам убедиться, что ты обладаешь необходимыми навыками для успешного прохождения
курса. А теперь в бой!

## Вводные инструкции
Задание должно быть реализовано только на стороне клиента с помощью Javascript (ES6), HTML, CSS,
без применения фреймворков или сторонних библиотек. Постарайся написать эффективный код, который легко
поддается модификациям и расширениям. Для этого можешь использовать любые подходы и парадигмы программирования.

## Задача

Построй двумерную сетку 50×50 из квадратных ячеек, каждая из которых может быть либо «живой», либо «мертвой».
Для построения можно использовать <div>, <td> или любой другой элемент на выбор. Ячейки белого цвета будем считать
живыми, ячейки черного цвета — мертвыми. В примерах мы используем 1 и 0 соответственно.
Начальная конфигурация сетки произвольная и должна меняться случайным образом при каждой перезагрузке страницы.

Для примера возьмем матрицу размера 5×5

```
00000
00000
01110
00000
00000
```

Полученная сетка живет по некоторым правилам: живые ячейки могут умирать, а мертвые заполняться новыми жителями.
Все преобразования происходят с некоторой периодичностью, назовем это циклом жизни.
Длительность цикла можешь установить на свое усмотрение.

## Правила преобразования сетки:

1. Каждая живая клетка с менее чем двумя живыми соседями умирает (underpopulation).
2. Каждая живая клетка с двумя или тремя живыми соседями доживает до следующего цикла.
3. Каждая живая ячейка с более чем тремя живыми соседями умирает (overcrowding).
4. Мертвая клетка с тремя живыми соседями становится живой клеткой (reproduction).

Рассмотрим сетку 5×5 и применим изложенные правила, чтобы смоделировать один цикл жизни:

```
00000           00000
00000           00100
01110 - tick -> 00100
00000           00100
00000           00000
```

##Вот и все!

Желаем тебе удачи в выполнении тестового и надеемся увидеть на курсе. Если тебя заинтересовали корни происхождения
этого задания, то рекомендуем посетить [википедию](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life).
По ссылке можно найти примеры устойчивых структур, которые помогут
понять, правильно ли работает твой алгоритм.

Ссылку на готовое задание нужно добавить в эту форму: https://forms.gle/4A47oSgZSgyhTASj9
