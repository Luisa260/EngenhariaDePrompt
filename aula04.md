# 1. Problema escolhido
Criar um programa que verifique se um número é primo.
# 2. Primeira interação (prompt vago)
# Prompt
Faça um código que diga se um número é primo.
# Resposta ruim (exemplo)
n = int(input())
if n % 2 == 0:
    print("Não é primo")
else:
    print("É primo")
# Problemas
❌ Incorreto (2 é primo e seria classificado errado)
❌ Não trata números menores que 2
❌ Lógica incompleta
❌ Sem explicação
❌ Sem organização
# 3. Prompt estruturado (prompt mestre)
# Agora aplicando: Persona + Contexto + Restrições + Formato
persona: Você é um professor de programação experiente e didático.

contexto: Preciso de um programa em Python que verifique se um número inteiro é primo. O código será usado por iniciantes que estão aprendendo lógica de programação.

restricoes:
  - O código deve ser simples e fácil de entender
  - Deve tratar números menores que 2 corretamente
  - Não usar bibliotecas externas
  - Deve ser eficiente para números até 1000
  - Incluir comentários explicando o passo a passo

formato:
  - Código em Python
  - Explicação antes do código
  - Exemplo de entrada e saída
# 4. Resultado refinado (ideal)
# Explicação
Um número primo é aquele que só pode ser dividido por 1 e por ele mesmo.
Para verificar isso, testamos divisões de 2 até a raiz quadrada do número.
# Código em Python
# Lê um número inteiro
n = int(input("Digite um número: "))

# Verifica se é menor que 2
if n < 2:
    print("Não é primo")
else:
    primo = True

    # Testa divisores de 2 até a raiz de n
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            primo = False
            break

    if primo:
        print("É primo")
    else:
        print("Não é primo")
# Exemplo
Entrada: 7
Saída: É primo
# O que melhorou?
✔ Código correto
✔ Explicação clara
✔ Estrutura organizada
✔ Tratamento de erros básicos
✔ Mais eficiente
✔ Fácil para iniciantes
