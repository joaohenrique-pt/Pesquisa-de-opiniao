# Programa de pesquisa de atendimento ao cliente

# Inicialização dos contadores
excelente = 0
bom = 0
ruim = 0

# Loop para 10 entrevistados
for i in range(1, 11):
    print(f"\nEntrevistado {i}")

    nome = input("Digite o nome: ")
    idade = int(input("Digite a idade: "))

    print("Avaliação do atendimento:")
    print("1 - EXCELENTE")
    print("2 - BOM")
    print("3 - RUIM")

    opiniao = int(input("Digite a opção (1, 2 ou 3): "))

    # Estrutura de decisão
    if opiniao == 1:
        excelente += 1
    elif opiniao == 2:
        bom += 1
    elif opiniao == 3:
        ruim += 1
    else:
        print("Opção inválida! Não contabilizada.")

# Resultado final
print("\n--- RESULTADO DA PESQUISA ---")
print(f"Quantidade de respostas 'EXCELENTE': {excelente}")
print(f"Quantidade de respostas 'BOM': {bom}")
print(f"Quantidade de respostas 'RUIM': {ruim}")
