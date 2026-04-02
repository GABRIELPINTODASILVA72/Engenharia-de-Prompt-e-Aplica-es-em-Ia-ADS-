# O Desafio

> Um problema de programação simples. O objetivo é criar um código funcional para calcular a média de notas de um aluno.

**prompt: imagine que voçê seja um professor de python e esta criando um codigo em python, com o objetivo de calcular a media  das notas dos alunos de uma escola, o codigo tem que ter a opção de adicionar as notas dos alunos e resultado final alinhado com os nomes com as informações se o aluno passou ou ele reprovou a media da escola e de 6 pontos as notas podem ser com virgulas entao oç sistema tem que suportar essas informacoes.**

# o codigo para calcular a media dos alunos


Perfeito! Vamos criar um código em Python que faça tudo isso: adicionar notas de alunos, calcular a média individual, informar se o aluno passou ou reprovou, e também calcular a média geral da escola. Vou considerar que a nota mínima para passar é 6. O sistema vai aceitar números com vírgulas (convertendo para ponto, já que Python usa ponto para float).

Aqui está um exemplo completo e comentado:
```python
# Lista para armazenar os alunos e suas notas
alunos = []

while True:
    nome = input("Digite o nome do aluno (ou 'sair' para finalizar): ")
    if nome.lower() == 'sair':
        break

    notas = []
    while True:
        nota_input = input(f"Digite a nota de {nome} (ou 'fim' para parar): ")
        if nota_input.lower() == 'fim':
            break
        # Substituir vírgula por ponto e converter para float
        try:
            nota = float(nota_input.replace(',', '.'))
            if 0 <= nota <= 10:
                notas.append(nota)
            else:
                print("Nota inválida. Digite um valor entre 0 e 10.")
        except ValueError:
            print("Entrada inválida. Digite um número válido.")

    if notas:  # só adiciona se tiver pelo menos uma nota
        media = sum(notas) / len(notas)
        situacao = "Aprovado" if media >= 6 else "Reprovado"
        alunos.append({"nome": nome, "notas": notas, "media": media, "situacao": situacao})

# Exibir resultados
print("\n--- RESULTADOS DOS ALUNOS ---")
for aluno in alunos:
    notas_formatadas = [f"{nota:.1f}" for nota in aluno['notas']]
    print(f"{aluno['nome']}: Notas: {notas_formatadas} | Média: {aluno['media']:.2f} | Situação: {aluno['situacao']}")

# Calcular média da escola
if alunos:
    media_escola = sum(aluno['media'] for aluno in alunos) / len(alunos)
    print(f"\nMédia da escola: {media_escola:.2f}")
else:
    print("Nenhum aluno cadastrado.")
```

✅ Funcionalidades desse código:
Permite adicionar vários alunos.
Permite adicionar várias notas por aluno.
Aceita notas com vírgulas (7,5 → 7.5).
Calcula a média individual e mostra se o aluno está aprovado ou reprovado.
Calcula a média da escola.
Resultado final exibido de forma organizada.

