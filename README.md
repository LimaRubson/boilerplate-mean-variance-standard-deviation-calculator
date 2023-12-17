# Mean-Variance-Standard Deviation Calculator

This is the boilerplate for the Mean-Variance-Standard Deviation Calculator project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-projects/mean-variance-standard-deviation-calculator

# My collaboration in the project:

O repositório contém um arquivo chamado mean_var_std.py que contém uma função chamada calculate. Essa função é projetada para realizar cálculos estatísticos em uma lista de 9 dígitos, considerando-os como elementos de uma matriz 3x3. A implementação faz uso da biblioteca NumPy para facilitar o processamento eficiente de operações matriciais e estatísticas.

## Assinatura da Função
```python
    import numpy as np

    def calculate(lst):
        # Implementação da função
```
## Entrada
A função calculate aceita um único parâmetro, lst, que deve ser uma lista contendo exatamente 9 elementos numéricos.

## Tratamento de Exceção
Se a lista de entrada não contiver exatamente 9 elementos, a função levanta uma exceção ValueError com a mensagem "List must contain nine numbers."

## Processamento da Matriz
A lista de entrada é convertida em uma matriz NumPy 3x3 usando np.array(lst).reshape(3, 3).
Diversos cálculos estatísticos são então realizados na matriz, incluindo média, variância, desvio padrão, máximo, mínimo e soma, tanto ao longo das linhas quanto das colunas.

## Formato do Resultado
A função retorna um dicionário contendo os resultados dos cálculos. O formato do dicionário é o seguinte:
```python
{
  'mean': [axis1, axis2, flattened],
  'variance': [axis1, axis2, flattened],
  'standard deviation': [axis1, axis2, flattened],
  'max': [axis1, axis2, flattened],
  'min': [axis1, axis2, flattened],
  'sum': [axis1, axis2, flattened]
}
```

## Exemplo de Uso
```python
# Exemplo de uso da função
result = calculate([0, 1, 2, 3, 4, 5, 6, 7, 8])
print(result)
```
