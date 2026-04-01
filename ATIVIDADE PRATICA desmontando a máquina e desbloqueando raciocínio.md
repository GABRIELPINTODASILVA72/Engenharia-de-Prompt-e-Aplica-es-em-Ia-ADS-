# Atividade Prática: Desmontando a Máquina

# Etapa 1 - Análise de Tokens (15 min):

> Acesse o OpenAl Tokenizer. Insira seu nome completo e a frase: "A engenharia de prompt otimiza LLMs". Registre quantos tokens foram gerados e observe a divisão morfológica.

FRASE: **gabriel pinto da silva engenharia de prompt otimiza llm.**

RESULTADO: **FICHAS: 14, PERSONAGEMS: 55.**








# Etapa 2 - Teste de Previsibilidade (20 min):

> No ChatGPT ou Gemini, envie o prompt:

> "O gato come...". Peça para listar as 3 palavras mais prováveis com justificativas lógicas. Simule diferentes temperaturas pedindo para a IA ser "muito criativa" vs "muito técnica".

PROMPT: **o gato come...  liste as 3 palavras mais prováveis com justificativas lógicas.**

RESULTADO: 
**ração**

> Justificativa: É a forma mais comum de alimentação de gatos domésticos. Em contextos cotidianos, essa é a continuação mais esperada.

**peixe**

> Justificativa: Culturalmente e popularmente, gatos são associados ao consumo de peixe, mesmo que não seja sempre a dieta principal.

**carne**

> Justificativa: Gatos são animais carnívoros, então “carne” é uma resposta biologicamente correta e plausível em termos gerais.


------------------------------------------------------------------------------------------------------------------------------------


# Atividade Prática: Desbloqueando o Raciocínio

# Etapa 3 - Raciocínio CoT (25 min):

> Teste o desafio: "Qual é a terceira letra da quinta palavra da frase 'O rato roeu a roupa do Rei de Roma'?" Se a IA errar, refaça o prompt forçando o passo a passo (Chain-of-Thought).

prompt: **Qual é a terceira letra da quinta palavra da frase 'O rato roeu a roupa do Rei de Roma'?**

RESULTADO: **Frase:**
**"O rato roeu a roupa do rei de roma"**

**Separando as palavras:**

**1 O**

**2 rato**

**3 roeu**

**4 a**

**5 roupa**

**6 do**

**7 rei**

**8 de**

**9 roma**

**A 5ª palavra é "roupa".**

**Agora, pegando a 3ª letra de "roupa":**

**r (1ª)**

**o (2ª)**

**u (3ª)**

**✅ Resposta: u**






# Entrega (GitHub):

> Crie um arquivo **aula03.md** no repositório da disciplina. Insira os prints das Etapas 1 e 3. Escreva uma breve conclusão refletindo sobre como a divisão de tokens influencia diretamente a resposta da IA.

REFLEXAO: **CASO TROQUE UM LETRA, A LLM TROCA AS PALAVRAS E O TEXTO GERADO DIFERENTE PARA CADA USUARIO, POR QUE ELE USA OS TOKENS PARA ANALIZAR E PROCESSAR A RESPOSTA.**







