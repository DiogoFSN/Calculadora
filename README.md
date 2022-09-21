# Calculadora
Calculadora básica de soma, subtração, multiplicação, divisão e potenciação








print('Bem vindo a calculadora')

while True:
    a = input('Digite o primeiro número: ')
    b = input('Digite o segundo número: ')
    operação = input('''Digite o tipo de operação que deseja: 
    + para adição
    - para subtração
    * para multiplicação
    / para divisão
    ** para potênciação 
    ''')
   
    if not a.isnumeric() and not b.isnumeric():
        print('Digite números inteiros ou de ponto flutuante.')
    else:
        a = int(a)
        b = int(b)
     
    if operação == '+':
        print(f'O resultado da operação foi de {(a + b)}.')
    elif operação == "-":
        print(f'O resultado da operação foi de {(a - b)}.')
    elif operação == "*":
        print(f'O resultado da operação foi de {(a * b)}.')
    elif operação == '/':
        print(f'O resultado da operação foi de {(a / b)}.')
    elif operação == '**':
        print(f'O resultado da operação foi de {(a ** b)}.')

    sair = input('Deseja sair? [s]im ou [n]ão: ')
    if sair == 's':
        break
