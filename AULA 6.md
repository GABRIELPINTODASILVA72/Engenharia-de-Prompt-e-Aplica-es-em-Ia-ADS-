# O Desafio

> Um problema de programação simples. O objetivo é criar um código funcional para calcular a média de notas de um aluno.

**prompt: imagine que voçê seja um professor de python e esta criando um codigo em python, com o objetivo de calcular a media  das notas dos alunos de uma escola, o codigo tem que ter a opção de adicionar as notas dos alunos e resultado final alinhado com os nomes com as informações se o aluno passou ou ele reprovou a media da escola e de 6 pontos as notas podem ser com virgulas entao oç sistema tem que suportar essas informacoes.**

# o codigo para calcular a media dos alunos


Perfeito! Vamos criar um código em Python que faça tudo isso: adicionar notas de alunos, calcular a média individual, informar se o aluno passou ou reprovou, e também calcular a média geral da escola. Vou considerar que a nota mínima para passar é 6. O sistema vai aceitar números com vírgulas (convertendo para ponto, já que Python usa ponto para float).

Aqui está um exemplo completo e comentado:
```python
# Lista para armazenar alunos
alunos = []

while True:
    nome = input("Digite o nome do aluno (ou 'sair' para finalizar): ")
    if nome.lower() == 'sair':
        break

    notas = []
    for i in range(6):
        nota_input = input(f"Digite a nota {i+1} de {nome} (ou 'fim' para parar): ")
        if nota_input.lower() == 'fim':
            break
        try:
            nota = float(nota_input.replace(',', '.'))
            if 0 <= nota <= 10:
                notas.append(nota)
                # Calcula média imediata
                media_atual = sum(notas) / len(notas)
                situacao_atual = "Aprovado" if media_atual >= 6 else "Reprovado"
                print(f"Média atual de {nome}: {media_atual:.2f} | Situação: {situacao_atual}")
            else:
                print("Nota inválida! Digite entre 0 e 10.")
        except ValueError:
            print("Entrada inválida! Digite um número.")

    if notas:
        # Calcula média final do aluno
        media_final = sum(notas) / len(notas)
        situacao_final = "Aprovado" if media_final >= 6 else "Reprovado"
        alunos.append({"nome": nome, "notas": notas, "media": media_final, "situacao": situacao_final})
    else:
        print(f"Nenhuma nota adicionada para {nome}.")

# Exibir resultados finais
print("\n--- RESULTADOS DOS ALUNOS ---")
for aluno in alunos:
    notas_formatadas = [f"{nota:.1f}" for nota in aluno['notas']]
    print(f"{aluno['nome']}: Notas: {notas_formatadas} | Média: {aluno['media']:.2f} | Situação: {aluno['situacao']}")

# Média da escola
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

