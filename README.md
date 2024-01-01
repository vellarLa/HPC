# HPC
- [lab-1. Matrix Multiplication](https://github.com/vellarLa/HPC/blob/main/HPC_1lab.ipynb)
Параллельный алгоритм реализован с использованием функции ядра.
Тип матриц - double, BLOCK_SIZE = 16, размер матриц задается в процессе выполнения программы
Алгоритм:
1) Считывание размерности матриц
2) Создаем массивы / выделяем память на CPU
3) Создаем массивы / выделяем память на GPU / выполняем проверку на успешное вделение памяти
4) Создание обработчиков событий для учета времени умножения на GPU
5) Заполнение матриц A и B на GPU рандомными значениями (0, 1)
6) Запуск функции ядра , выполнение умножения на GPU
7) Синхронизация устройств
8) Копирование матриц на CPU
9) Умножение матриц на CPU
10) Вывод результатов
11) Освобождение памяти GPU и CPU
Результаты, программный код и комментарии приведены по ссылке.

- [lab-2. Matrix Multiplication](https://github.com/vellarLa/HPC/blob/main/HPC_2lab.ipynb)
Параллельный алгоритм реализован с использованием функции ядра.
Тип векторов - double, BLOCK_SIZE = 512, GRID_SIZE = 1024; размер матриц задается в процессе выполнения программы
Алгоритм:
1) Считывание размерности векторов
2) Создаем массивы / выделяем память на CPU
3) Создаем массивы / выделяем память на GPU / выполняем проверку на успешное вделение памяти
4) Создание обработчиков событий для учета времени сложения на GPU
5) Заполнение векторов A и B на СPU рандомными значениями (0, 1)
6) Копировние векторов с хоста на девайс
7) Запуск функции ядра , выполнение сложения на GPU
8) Синхронизация устройств
9) Копирование  на CPU
10) Умножение матриц на CPU
11) Вывод результатов
12) Освобождение памяти GPU и CPU
Результаты, программный код и комментарии приведены по ссылке.

- [lab-3. Pi-value Calculation, 1 point](https://github.com/vellarLa/HPC/blob/main/HPC_3lab.ipynb)
Параллельный алгоритм расчета значения pi.
