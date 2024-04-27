# QuickResults_GIT

## Описание задачи

В задаче обработки измерений радара, сопровождающего тесную группу низколетящих целей, ассоциация замеров с траекториями может быть выполнена множеством различных комбинаций. Вам необходимо найти три лучшие комбинации, которые обеспечивают оптимальную ассоциацию замеров к траекториям.

## Техническое окружение

Этот проект предполагает наличие Python 3 и следующих библиотек:

- numpy
- pandas
- scipy (или иной инструмент для оптимизации)

## Запуск алгоритма

Чтобы запустить алгоритм, выполните следующие шаги:

1. Склонируйте этот репозиторий:
    
    bash
    
    Copy code
    
    `git clone <ваша_ссылка>`
    
2. Перейдите в директорию проекта:
    
    bash
    
    Copy code
    
    `cd <имя_проекта>`
    
3. Убедитесь, что все необходимые библиотеки установлены:
    
    bash
    
    Copy code
    
    `pip install -r requirements.txt`
    
4. Запустите основной скрипт:
    
    bash
    
    Copy code
    
    `python main.py`
    

## Формат входных данных

На вход алгоритму подается матрица совместности траекторий в формате CSV. Пример файла:

Copy code

`0,1,0,1,... 1,0,1,0,... 0,1,0,1,...`

Также требуется вектор весов траекторий, который также представлен в формате CSV. Пример файла:

Copy code

`1.0,0.8,0.9,1.2,...`

## Формат выходных данных

На выходе алгоритм генерирует матрицу топ-5 глобальных гипотез с их весами в формате CSV. Пример файла:

Copy code

`1,0,1,0,... 0,1,0,1,... 1,0,1,0,...`

## Ограничения

- Максимальное время работы алгоритма для матрицы 28х28 - 1 секунда.
- Эксперты оценивают время работы алгоритма на разных матрицах для траекторий, уделяя особое внимание точности, скорости и визуализации.
