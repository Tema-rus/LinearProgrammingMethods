# ExpressionParser

Класс для анализа и разбора линейных выражений в Python.

## Описание

`ExpressionParser` - это класс, предназначенный для анализа и разбора линейных математических выражений. Он извлекает информацию о переменных, их коэффициентах и знаке неравенства (или стремления) из входного выражения.

## Установка

Для использования `ExpressionParser` в вашем проекте, вы можете просто скопировать файл `expression_parser.py` и импортировать класс в свой код.

```python
from expression_parser import ExpressionParser
```
## Пример использования

Пример использования `ExpressionParser`:


```python
target_expression = input('Введите целевую функцию: ')
target_parser = ExpressionParser(target_expression)
print(f'\n{target_parser.constant = }\n{target_parser.sign = }\n{target_parser.variables = }\n')

num_constraints = int(input('Введите количество ограничений: ')

constraint_parsers = []
for i in range(num_constraints):
    constraint = input(f'Введите ограничение {i + 1}: ')
    constraint_parser = ExpressionParser(constraint)
    constraint_parsers.append(constraint_parser)
    print(f'\n{constraint_parser.constant = }\n{constraint_parser.sign = }\n{constraint_parser.variables = }\n')
```
