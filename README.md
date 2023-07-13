# Проект 1. Обработка клиентской базы hh.ru

## Оглавление  
[1. Описание проекта](README.md#Описание-проекта)  
[2. Какой кейс решаем?](README.md#Какой-кейс-решаем)  
[3. Краткая информация о данных](README.md#Краткая-информация-о-данных)  
[4. Этапы работы над проектом](README.md#Этапы-работы-над-проектом)  
[5. Результаты](README.md#Результаты)    
[6. Выводы](README.md#Выводы)
[7. Графики](README.md#Графики)

### Описание проекта    
Учебный проект по обработке части реального датасета. В датасете резюме соискателей работы с сайта hh.ru.

:arrow_up:[к оглавлению](README.md#Оглавление)


### Какой кейс решаем?    
Задачами проекта являются анализ, преобразование и очистка данных, для дальнейшего обучения модели по определению предлагаемой зарплаты соискателям, не указавшим данную информацию в своих резюме.

**Метрика качества**     
- все ключевые признаки должны быть преобразованы в вид, позволяющий анализировать их автоматизировано;
- провести разведывательный анализ данных;
- очистить данные от дубликатов, выбросов и пропусков с минимальными потерями.

**Что практикуем**     
- закрепляем знания по работе с DataFrame;
- тренируемся выявлять взаимосвязи между признаками на реальном кейсе;
- практикуем построение графиков и очистку данных.


### Краткая информация о данных
Датасет содержит 12 признаков и 44744 строки.
Все строки содержат в себе данные из резюме, заполненных соискателями с сайта hh.ru.
Часть признаков содержит в себе текст, заполненный в частично структурированной, но требующей преобразования форме.
К примеру, один из таких признаков "Пол, возраст" - оба параметра, содержащиес в признаке, интересуют нас при исследовании, но в таком виде работать с ними затруднительно.
Существуют и другие признаки, содержащие в себе до 5 параметров, которые хотелось бы разделить или преобразовать.
Отдельные признаки содержат в себе много ненужной для обучения модели информации. К примеру, перечисление всех мест работы в признаке "Опыт работы".
  
:arrow_up:[к оглавлению](README.md#Оглавление)


### Этапы работы над проектом  
1. Базовый анализ структуры данных
2. Преобразование данных
3. Разведывательный анализ
4. Очистка данных
  
:arrow_up:[к оглавлению](README.md#Оглавление)


### Результаты:  
В результате работы 7 признаков, содержащих важную, но представленную в неудобной форме информацию, переработаны в 18 новых признаков, доступных для дальнейшего обучения.
Выявлены признаки, в наибольшей степени влияющие на предпочтения соискателей относительно их будущей зарплаты.
Датасет очищен от дупликатов и выбрасов. Часть пропусков заполнена константами, некоторые строки с пропусками удалены.
Итоговая форма датасета (44482, 23), из чего следует, что потеря данных составила 262 записи или 0,59%.

:arrow_up:[к оглавлению](README.md#Оглавление)


### Выводы:  
В ходе работы над проектом были закреплены знания по обработке, преобразованию, очистке и заполнению данных в DataFrame, а также по построению графиков и анализу имеющейся информации.
Данный кейс продемонстрировал принципы применения обработки данных в реальной жизни, помог лучше понять возникающие сложности и пути их решения.
  
:arrow_up:[к оглавлению](README.md#Оглавление)



### Графики:
В ходе работы над проетом были построены графики с использование библиотеки plotly. 
К сожалению, технические возможности Github не позволяют продемонстировать данные графики непосредственно из юпитер-ноутбука.
Если вам интересно с ними ознакомиться, сделать это можно [здесь](https://github.com/AndKober/Project_1/tree/master/plotly)