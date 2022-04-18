# Проект 0. Угадай число

## Оглавление  
[1. Описание проекта](.README.md#Описание-проекта)  
[2. Какой кейс решаем?](.README.md#Какой-кейс-решаем)  
[3. Краткая информация о данных](.README.md#Краткая-информация-о-данных)  
[4. Этапы работы над проектом](.README.md#Этапы-работы-над-проектом)  
[5. Результат](.README.md#Результат)    
[6. Выводы](.README.md#Выводы) 

### Описание проекта    
Угадать загаданное компьютером число за минимальное число попыток.

:arrow_up:[к оглавлению](_)


### Какой кейс решаем?    
Нужно написать программу, которая угадывает число за минимальное число попыток

**Условия соревнования:**  
- Компьютер загадывает целое число от 0 до 100, и нам его нужно угадать. Под «угадать», подразумевается «написать программу, которая угадывает число».
- Алгоритм учитывает информацию о том, больше ли случайное число или меньше нужного нам.

**Метрика качества**     
Результаты оцениваются по среднему количеству попыток при 1000 повторений

**Что практикуем**     
- Учимся писать хороший код на python.
- Учимся работать с IDE.
- Учимся работать с GitHub.


### Краткая информация о данных
....
  
:arrow_up:[к оглавлению](.README.md#Оглавление)


### Этапы работы над проектом  
1. Первым делом импортируем библиотеку numpy и создаём функцию, которая принимает аргумент число "int". Это число и требуется угадать.
2. Внутри функции создаём счётчик попыток, две переменные "start_of_range", "end_of_range" и бесконечный цикл "while". В цикле с помощью "np.random.rendit" перебираем случайные числа, сравнивая их с истинным числом. Корректируем диапазон с помощью переменных. При совпадении прерываем цикл.
3. Взвращаем счётчик попыток.
4. Создаём вторую функцию, которая будет выводить среднее количество угадываний из 1000 повторений. Аргументом функции являяется предыдущая функция.
5. Внутри этой функции создаём список тысячи случайных чисел от 1 до 100.
6. Через цикл "for" прогоняем список из тысячи случайных чисел через первую функцию. В отдельный список добавляем результат работы первой функции, а именно количество попыток угадывания.
7. Вычисляем среднее значение списка с количеством попыток с помощью "np.mean".
8. Возвращаем среднее значение.

:arrow_up:[к оглавлению](.README.md#Оглавление)


### Результаты:  
В результате мы имеем две функции. Одна угадывает заданное число и возвращает наименьшее колличество попыток угадываний. Вторая функция прорабатывает первую функцию 1000 раз и выводит среднее количество попыток, требуемое для угадывания того или иного числа.

:arrow_up:[к оглавлению](.README.md#Оглавление)


### Выводы:  
Итог работы обеих функций показывает, что среднее количество попыток из тысячи повторений, необходимое для поиска того или иного числа в диапазоне от 1 до 100, составляет 7.

:arrow_up:[к оглавлению](.README.md#Оглавление)


Если информация по этому проекту покажется вам интересной или полезной, то я буду очень вам благодарен, если отметите репозиторий и профиль ⭐️⭐️⭐️-дами