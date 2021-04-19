# Вступительное задание

Привет! Если ты читаешь этот текст — ты на половине пути к поступлению на курс front-end middle. Мы очень хотим чтоб курс был максимально полезным для обучающихся по этому мы просим тебя выполнить небольшое вступительное задание. Это позволит нам убедится что ты обладаешь всеми необходимыми навыками для успешного прохождения курса. А теперь в бой!

## Задание

### Вводные инструкции
Задание должно быть реализовано только на стороне клиента с использованием Javascript (ES6),
HTML, CSS, **без использования фреймворков или сторонних библиотек**. 
Постарайся написать эффективный код, который легко поддается модификациям и расширениям. 
Для этого ты можешь использовать любые подходы и парадигмы программирования, которые захочешь.

### Задача

Построй двумерную сетку 50x50 из квадратных ячеек, каждая из этих ячеек может быть либо "живой", либо "мертвой".
Для построения можно использовать `<div>`, `<td>` либо любой другой элемент, который ты выберешь. 
Ячейки белого цвета будем считать "живыми", ячейки черного цвета — "мертвыми".
В примерах мы используем 1 и 0 соответственно.
Начальная конфигурация сетки произвольная и должна меняться случайным образом при каждой перезагрузке страницы.

Для примера возьмем матрицу размера 5 на 5

```
00000
00000
01110
00000
00000
```

Полученная сетка живет по некоторым правилам, живые ячейки могут умирать, а мертвые заполняться новыми жителями.
Все преобразования происходят с некоторой периодичностью, назовем это _циклом жизни_.
Длительность цикла ты можешь установить на свое усмотрение.

### Правила преобразования сетки:

1. Каждая живая клетка с менее чем двумя живыми соседями умирает (underpopulation).
2. Каждая живая клетка с двумя или тремя живыми соседями доживает до следующего цикла.
3. Каждая живая ячейка с более чем тремя живыми соседями умирает (overcrowding).
4. Мертвая клетка с тремя живыми соседями становится живой клеткой (reproduction).

Рассмотрим сетку 5 на 5 и применим изложенные правила, чтоб смоделировать один цикл жизни:

```
00000           00000
00000           00100
01110 - tick -> 00100
00000           00100
00000           00000
```

### Вот и все!

Желаем тебе удачи в написании тестового задания и надеемся увидеть на курсе.
Если тебя заинтересовали корни происхождния этого задания то рекомендуем посетить [википедию](https://ru.wikipedia.org/wiki/%D0%98%D0%B3%D1%80%D0%B0_%C2%AB%D0%96%D0%B8%D0%B7%D0%BD%D1%8C%C2%BB). По ссылке ты можешь найти примеры устойчивых структур, которые помогут тебе понять правильно ли работает твой алгоритм.


