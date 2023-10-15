# находим среднее значение
def find_average(x):
    return sum(x) / len(x)


# находим размах
def find_range(x):
    x_copy = sorted(x)
    return abs(x_copy[-1] - x_copy[0])

# находим медиану
def find_median(x):
    if len(x) % 2 == 0:
        return (x[len(x) // 2] + x[len(x) // 2 -1]) / 2
    else:
        return x[len(x) // 2]


# находим дисперсию в генеральной совокупности
def find_general_variance(x, x_average):
    variance = 0
    for i in x:
        variance += (i - x_average) ** 2
    return variance / len(x)


# находим дисперсию в выборке
def find_subgeneral_variance(x, x_average):
    variance = 0
    for i in x:
        variance += (i - x_average) ** 2
    return variance / (len(x) - 1)


# возвращаем квадрат из числа
def get_sqrt(x):
    return x ** 0.5

Для подзабывших питон шпаргалка:

import statistics

ls = 1, 5, 2, 7, 1, 9, 3, 8, 5, 9

mean = sum(ls) / len(ls)
print(mean, statistics.mean(ls))

variance = sum((x - mean) ** 2 for x in ls) / (len(ls) - 1)
print(variance, statistics.variance(ls))

stdev = variance ** (1 / 2)
print(stdev, statistics.stdev(ls))

import numpy as np
from scipy import stats

data = input().split()
data = np.array(data, dtype=int)
print(data)

M = np.mean(data)  # среднее сзначение
mode = stats.mode(data)   # мода
median = np.median(data)  # медиан
R = np.max(data) - np.min(data)  # размах
D = np.var(data)  # дисперсия
sd = np.std(data)  # стандартное отклонение

print(f'Среднее значение: {M}, мода: {mode[0]}, медиан: {median}, размах: {R}, дисперсия: {D}, стандартное отклонение: {sd}')