# intelligent_information_processing_technologies
# Технологиии интеллектуальной обработки информации

### Базы знаний

**Цель** Реализация своей базы знаний на python

**задачи**
- повторить _git_ (создание репозитория, gitignore, коммиты и пр)
- повторить _docker_ (Dockerfile best practices, создание образов, запуск контейнеров)
- повторить _markdown_ (синтаксис, что должно быть в readme.md)
- повторить основы _python_ (функции, циклы, операторы)

**Задачи**
(_TODO_)


### Линейная регрессия, полиномиальная регрессия, метод градиентного спуска

Рекомендуется использоваться Ubuntu 20.04 с установленными:
- python3
- numpy
- matplotlib
- sklearn

**Цель** Реализация и оптимизация метода градиентного спуска, решение задач регрессии

**задачи**
- освоить базовые операции _numpy_ (импорт/экспорт numpy array, перемножение матриц)
- решение задач регрессии с помощью _polyfit_
- освоить построение графиков в _matplotlib_

**Задачи**
1. Реализовать точное решение задачи поиска решения задачи регрессии (в матричном виде через обратную матрицу - использовать _pinv_, а не _inv_)

```python
def linear_regression_exact(filename):
    print("Ex1: your code here - exact solution usin invert matrix")
    return
```

2. Полиномиальная регрессия с помощью _numpy polyfit_

```python
def polynomial_regression_numpy(filename):
    print("Ex2: your code here")
    time_start = time()
    print("Ex2: your code here")
    time_end = time()
    print(f"polyfit in {time_end - time_start} seconds")
```

3. Реализовать самостоятельно метод градиентного спуска

- **alpha** - скорость градиентного спуска (скаляр)
- **theta** - текущие параметры модели (shape is 1 х N)
- **J(theta)** - функция потерь (сумма квадратов отклонений), которую минимизируем
- **dJ(theta)** - градиент, является вектором той же размерности, что и **theta** (1 x N)
- x и y - тоже вектора/матрицы

Расчет шага градиентного спуска (все аргументы - векторы)
```python
def gradient_descent_step(dJ, theta, alpha):
    print("your code goes here")

    return(theta_new)
```

Расчет градиентов J для каждой из реализаций градиентного спуска (постарайтесь обойтись без циклов - чисто на матричных и векторных операциях numpy). Можно считать численно, можно использовать аналитическое выражение для значения частной производной.

```python
# get gradient over all xy dataset - gradient descent
def get_dJ(x, y, theta):
    d_theta = theta
    print("your code goes here - calculate new theta")
    return d_J   

# get gradient over all minibatch of size M of xy dataset - minibatch gradient descent
def get_dJ_minibatch(x, y, theta, M):
    d_theta = theta
    print("your code goes here - calculate new theta")
    return d_J     

# get gradient over all minibatch of single sample from xy dataset - stochastic gradient descent
def get_dJ_sgd(x, y, theta):
    d_theta = theta
    print("your code goes here - calculate new theta")
    return d_J    
```


В цикле проходите и минимизируете J с помощью функции

```python
def minimize(theta, x, y, L):
```

