# Algoritmo MaxMin Select 
O algoritmo de seleção simultânea (MaxMin Select) pode ser implementado de forma recursiva, utilizando a técnica de divisão e conquista. O problema é dividido em subproblemas menores que são resolvidos recursivamente, e seus resultados são combinados para encontrar o maior e o menor elementos com eficiência. Esse método reduz o número de comparações necessárias em comparação com uma abordagem ingênua.

## Como funciona o algoritmo MaxMin Select?
### Entrada do Usuário:
O programa solicita ao usuário que insira uma sequência de números separados por espaços. A entrada é convertida em uma lista de inteiros usando map(int, user_input.split()).
### Validação:
Se a entrada estiver vazia ou contiver valores inválidos (não numéricos), o programa exibe uma mensagem de erro.
###Execução do Algoritmo:
A função max_min_select é chamada com a lista de números fornecida pelo usuário. O menor e o maior número são calculados e exibidos.

## Ideia principal
O código implementa o algoritmo de seleção simultânea do maior e menor elemento (MaxMin Select) utilizando a abordagem de divisão e conquista. A ideia principal é dividir a sequência de números em partes menores, calcular o menor e o maior elemento em cada parte e, em seguida, combinar os resultados para obter o menor e o maior elementos globais da sequência.

A lógica segue o princípio de dividir o problema em subproblemas menores, resolvê-los recursivamente e combinar as soluções para obter o resultado final. Esse método reduz o número de comparações necessárias para encontrar o menor e o maior elemento simultaneamente, tornando-o mais eficiente do que métodos tradicionais.

## Lógica de Como foi Implementado
Linha 9-14: Caso base, em que, se a lista tem apenas um elemento, retorna esse elemento como sendo tanto o menor quanto o maior. Se a lista tem dois elementos, compara diretamente os dois e retorna o menor e o maior.

Linha 17: Divide a lista ao meio, separando-a em duas partes: metade esquerda (arr[:mid]) e metade direita (arr[mid:]).

Linha 18-19: Aplica recursivamente o algoritmo max_min_select nas duas metades da lista para encontrar o menor e o maior elemento em cada metade.

Linha 22-23: Combina os resultados das duas metades. O menor elemento global é o menor entre os menores das duas metades, e o maior elemento global é o maior entre os maiores das duas metades.

Linha 25: Retorna uma tupla contendo o menor e o maior elemento encontrados na sequência.

## Dependências
Nenhuma 

## Como Roda o Projeto
Passo 1: 
Entre no arquivo "Code/.venv/Lib/site-packages/pip/__main__.py" utilizando sua IDE de preferência

Passo 2: 
Rode o arquivo.

## Versão do Python
Este projeto foi desenvolvido na versão 3.13.0 do Python.

##Explicação das funções
### Arquivo: 
__main__.py
### Objetivo: 
Este arquivo principal realiza a seleção simultânea do maior e menor elemento de uma sequência de números utilizando o algoritmo MaxMin Select com abordagem de divisão e conquista. Ele também permite que o usuário insira os números da sequência.
### Descrição das funções:
max_min_select(arr)
Recebe uma lista de números e utiliza o método de divisão e conquista para encontrar simultaneamente o menor e o maior elemento da lista.
#### Parâmetros:
arr: Lista de números inteiros ou reais fornecida pelo usuário.
#### Retorno:
Uma tupla contendo dois valores:
- O menor elemento da lista.
- O maior elemento da lista.

# Relatório Técnico 

## Fluxo de Controle da Função 

1. Início da Função
2. Verificação da condição len(arr) == 1
   - Se verdadeiro: retorna arr[0], arr[0]
   - Se falso: Passa direto para a próxima iteração
3. Verificação da condição len(arr) == 2
   - Se verdadeiro: retorna min(arr[0], arr[1]), max(arr[0], arr[1])
   - Se falso: Passa direto para a próxima iteração
4. Inicializa a variável mid
5. Inicializa as variáveis left_min e left_max
6. Inicializa as variáveis right_min e right_max
7. Inicializa a variável overral_min
8. Inicializa a variável overral_max
9. Retorna o valor mínimo e máximo

Nós: 
1. Início da Função
2. Verificação do if
3. Ação dentro do if
4. Verificação do if
3. Ação dentro do if
5. Inicializaçao de mid
6. Inicialização das variáveis left_min e left_max
6. Inicialização das variáveis right_min e right_max
7. Inicialização da variável overral_min
8. Inicialização da variável overral_max
9. Retorno final

-----------------------------Falta fazer daqui pra baixo

Arestas: 
1. Inicio do nó para verificação do if
2. Verificação do If para ação dentro do if
3. Verificação do If para retorno final
4. Ação dentro do if para inicialização de n
5. Inicialização de n para inicialização de m
6. Inicialização de m para inicialização das variáveis high_x e low_x
7. Inicalização das variáveis high_x e low_x para a Inicialização das variáveis high_y e low_y
8. Inicialização das variáveis high_y e low_y para inicialização da variável z0
9. Inicialização da variável z0 para inicialização da variável z1
10. Inicialização da variável z1 para inicialização da variável z2
11. Inicialização da variável z2 para retorno final

![image](https://github.com/user-attachments/assets/484c115e-989b-440d-921a-9b230a38165a)

### Complexidade Ciclomática = E - N + 2P = 11 - 10 + 2*1 = 3 

### Complexidade Assintótica

**Complexidade temporal:** 
- Melhor caso: O(1)
- Caso Médio: O(n^{1.585})
- Pior caso: O(n^{1.585})

**Complexidade Espacial:**
- Melhor caso: O(1)
- Caso Médio: (O(\log n)
- Pior Caso: O(\log n)
