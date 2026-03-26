# ATIVIDADE 2 

# Tema escolhido

  Estruturas de repetição


O prompt mestre inicial que você utilizou.


variação 1:crie uma calculadora e deixe tudo em markdown ate o código.


variação 2:caso você fosse um programador e esta criando uma calculadora em python coloque tudo em markdown ate o código. 


variação 3:você e um programador renomado e esta criando um código de calculadora utilizando a linguagem de python coloque tudo em
markdown ate o código.



# código 1:# Calculadora Simples em Python

## Descrição
Uma calculadora básica que realiza as quatro operações: soma, subtração, multiplicação e divisão.

## Código

```python
# Calculadora simples

def soma(a, b):
    return a + b

def subtracao(a, b):
    return a - b

def multiplicacao(a, b):
    return a * b

def divisao(a, b):
    if b == 0:
        return "Erro: divisão por zero"
    return a / b

print("Escolha a operação:")
print("1 - Soma")
print("2 - Subtração")
print("3 - Multiplicação")
print("4 - Divisão")

opcao = input("Digite o número da operação: ")

num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

if opcao == "1":
    print("Resultado:", soma(num1, num2))
elif opcao == "2":
    print("Resultado:", subtracao(num1, num2))
elif opcao == "3":
    print("Resultado:", multiplicacao(num1, num2))
elif opcao == "4":
    print("Resultado:", divisao(num1, num2))
else:
    print("Opção inválida")
```
# código 2:# Calculadora em Python

```python
# Função para adicionar dois números
def adicionar(a, b):
    return a + b

# Função para subtrair dois números
def subtrair(a, b):
    return a - b

# Função para multiplicar dois números
def multiplicar(a, b):
    return a * b

# Função para dividir dois números
def dividir(a, b):
    if b == 0:
        return "Erro: Divisão por zero!"
    return a / b

# Função principal da calculadora
def calculadora():
    print("=== Calculadora em Python ===")
    
    while True:
        print("\nSelecione a operação:")
        print("1 - Adição")
        print("2 - Subtração")
        print("3 - Multiplicação")
        print("4 - Divisão")
        print("5 - Sair")
        
        escolha = input("Digite o número da operação desejada: ")
        
        if escolha == '5':
            print("Encerrando a calculadora. Até logo!")
            break
        
        if escolha in ['1', '2', '3', '4']:
            try:
                num1 = float(input("Digite o primeiro número: "))
                num2 = float(input("Digite o segundo número: "))
            except ValueError:
                print("Erro: Digite apenas números válidos!")
                continue
            
            if escolha == '1':
                print(f"Resultado: {adicionar(num1, num2)}")
            elif escolha == '2':
                print(f"Resultado: {subtrair(num1, num2)}")
            elif escolha == '3':
                print(f"Resultado: {multiplicar(num1, num2)}")
            elif escolha == '4':
                print(f"Resultado: {dividir(num1, num2)}")
        else:
            print("Opção inválida! Tente novamente.")

# Executa a calculadora
if __name__ == "__main__":
    calculadora()
 ````
# código 3:# Calculadora Simples em Python

````python
# Autor: Programador Renomado
# Linguagem: Python 3

def soma(a, b):
    """Retorna a soma de dois números"""
    return a + b

def subtracao(a, b):
    """Retorna a subtração de dois números"""
    return a - b

def multiplicacao(a, b):
    """Retorna a multiplicação de dois números"""
    return a * b

def divisao(a, b):
    """Retorna a divisão de dois números, tratando divisão por zero"""
    if b == 0:
        return "Erro: Divisão por zero!"
    return a / b

def calculadora():
    """Função principal da calculadora"""
    print("Bem-vindo à Calculadora Python!")
    while True:
        print("\nEscolha a operação:")
        print("1 - Soma")
        print("2 - Subtração")
        print("3 - Multiplicação")
        print("4 - Divisão")
        print("0 - Sair")
        
        escolha = input("Digite sua escolha (0-4): ")
        
        if escolha == "0":
            print("Saindo da calculadora. Até mais!")
            break
        
        if escolha in ("1", "2", "3", "4"):
            try:
                num1 = float(input("Digite o primeiro número: "))
                num2 = float(input("Digite o segundo número: "))
            except ValueError:
                print("Erro: Por favor, digite apenas números válidos!")
                continue
            
            if escolha == "1":
                print(f"Resultado: {soma(num1, num2)}")
            elif escolha == "2":
                print(f"Resultado: {subtracao(num1, num2)}")
            elif escolha == "3":
                print(f"Resultado: {multiplicacao(num1, num2)}")
            elif escolha == "4":
                print(f"Resultado: {divisao(num1, num2)}")
        else:
            print("Opção inválida! Digite um número de 0 a 4.")

# Executa a calculadora
if __name__ == "__main__":
    calculadora()

````
 
#As respostas geradas pelo LLM para cada versão: CHAT GPT




Uma reflexão crítica (5–10 linhas) sobre:



Como diferentes instruções mudaram a resposta.
Qual versão foi mais útil para o aprendizado.
Como você poderia aplicar essa técnica em situações reais de programação.
