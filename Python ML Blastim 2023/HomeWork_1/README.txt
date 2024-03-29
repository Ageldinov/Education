**Задание 1:**

Напишите функцию, которая будет принимать на вход экспрессии гена, семплировать их них выборки размера `sample_size`, считать среднюю экспрессию и повторять это `n_samples` раз. Примените эту функцию к экспрессиям гена `TMCC1` в обоих клеточных типах, визуализируйте их. Отличаются ли средние экспрессии данного гена у этих клеточных типов?

**Задание 2:**
Напишите функцию для проверки того, что доверительные интервалы пересекаются. На лекции мы тестировали гипотезы для равенства среднего выборки заданному числу и проверяли, попало ли оно в границы этого интервала или нет, если оно оказывалось за ними, то мы говорили, что средние отличаются. Здесь же мы имеем дело с двумя выборками, поэтому будем проверять, пересекаются ли доверительные интервалы, и, если нет, то говорить о том, что средние в выборках отличаются.

**Задание 3:**
Давайте теперь применим для той же задачи `z-критерий`. Будем считать, что в данном случае $\alpha$ = 0.05, и если полученное `p-value` будет меньше, то экспрессия генов значимо отличается.

**Задание 4:**
Теперь пришла пора оформить все ваши старания в виде программы. Напишите программу (можно просто функцию), которая принимает на вход следующие аргуметры:

1. `first_cell_type_expressions` &ndash; таблица с экспрессиями генов для одного клеточного типа;
2. `second_cell_type_expressions` &ndash; таблица с экспрессиями генов для второго клеточного типа;

Как читать данные при помощи пандаса мы уже знаем, осталось понять, как записывать результаты.
