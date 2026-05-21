# **CALCULADORA SIMPLES**


```python
# a calculadora tem como principal requisito FUNCIONAR,
# a calculadora ira ter as principais operacoes, soma , subtracao
# , divisao e multiplicacao.



# calculadora simples

try: # se der erro vai execultar o except direto

  num1 = float(input("digite o primeiro num")) # pede um num
  num2 = float(input("digite o segundo num")) # pede outro num
  operacao = int(input("digite 1 para soma, 2 para subtracao, 3 para multiplicacao , 4 para divisao")) # pede a operacao

#-------------------------------------
  if operacao == 1:  # se for 1
    soma = (num1 + num2)  # ele soma
    print(soma)  # printa na tela
#-------------------------------------
  if operacao == 2:  # se for 2
    sub = (num1 - num2)  # ele subtrai
    print(sub)  # printa na tela
#-------------------------------------
  if operacao == 3:  # se for 3
    mult = (num1 * num2) # ele multiplica
    print(mult)  # printa na tela
#-------------------------------------
  if operacao == 4:  # se for 4
    divisao = (num1 / num2)  # ele divide
    print(divisao) # printa na tela

#-----------------------------------------------------
except:  # caso try observar que vai dar erro ele manda esse codico execultar
  print("isto nao pode ser processado")


finally: # mesmo com erro ou sem erro ele execulta
  print("programa finalizado ")
