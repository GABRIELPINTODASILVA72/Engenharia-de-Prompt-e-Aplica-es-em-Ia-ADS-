# O Desafio:

> Transformar uma instrução vaga em um Prompt Mestre estruturado.

 > Ferramentas: ChatGPT ou GitHub Copilot.

 # A Tarefa :

> 1. Escolha um problema de código simples ou necessidade de documentação de um projeto pessoal.

prompt simples: **ME AJUDE NOS CODIGOS WHILE E FOR DO PYTHON**


> 2. Crie uma primeira interação (vaga) e documente a resposta ruim.

prompt 1° interação: 🔁 while

Repete enquanto a condição for verdadeira:

```python

i = 1
while i <= 5:
    print(i)
    i += 1
```

🔄 for


Percorre uma sequência:
```python
for i in range(1, 6):
    print(i)

```

🧠 Diferença

while → quando não sabe quantas vezes
for → quando já sabe ou tem lista



> 3. Aplique a Equação do Prompt (Persona + Contexto + Restrições + Formato).

prompt 2: **IMAGINE QUE VOCE SEJA UM PROFESSOR MUITO BOM EM PROGRAMAR PYTHON, E ESTA ME EMCINANDO OS CODIGOS WHILE E FOR, MOSTRANDO PASSO A PASSO DA AULA.**

> 4. Refine iterativamente até obter o resultado perfeito em formato YAML ou Markdown.


RESULTADO: 

🧠 Aula 1: Entendendo o while
📌 O que é o while?

O while é um laço de repetição. Ele executa um bloco de código enquanto uma condição for verdadeira.


🧾 Estrutura básica:
````

while condição:
````

# código que será repetido
✅ Exemplo 1:
```
Contar de 1 até 5
contador = 1

while contador <= 5:
    print(contador)
    contador += 1
```

🔍 Passo a passo:

Criamos uma variável contador = 1
O while pergunta:
👉 "contador é menor ou igual a 5?"
Se for verdade:
imprime o número
soma 1 ao contador
Repete isso até chegar em 6
📊 Resultado:
1 

2

3

4

5

⚠️ Cuidado importante!

Se você esquecer de atualizar a variável, o loop vira infinito 😱

Exemplo errado:
```
while True:
    print("Nunca para!")

```
🔁 Aula 2: Entendendo o for
📌 O que é o for?

O for é usado para percorrer sequências (listas, números, textos).

🧾 Estrutura básica:

```
for variável in sequência:
    # código
```
✅ Exemplo 2: Contar de 1 até 5 com for
```
for numero in range(1, 6):
   print(numero)
```
🔍 Passo a passo:
range(1, 6) gera números de 1 até 5
O for pega cada número
Coloca na variável numero
Executa o print
📊 Resultado:
1

2

3

4

5

🔥 Comparando while vs for
while 🧠	for 🚀
Usa condição	Usa sequência
Mais flexível	Mais simples
Pode dar loop infinito	Mais seguro
🎯 Exemplo prático (vida real)
🧮 Somar números de 1 a 5 com for:

```
soma = 0

for numero in range(1, 6):
    soma += numero

print(soma)
```
👉 Resultado: 15

🧮 Mesmo exemplo com while:

```
soma = 0
contador = 1

while contador <= 5:
    soma += contador
    contador += 1

print(soma)

```
🧪 Exercício para você tentar 👇

👉 Tente fazer um programa que:

Mostre números de 10 até 1 (contagem regressiva)

💡 Dica:

Use while ou for







