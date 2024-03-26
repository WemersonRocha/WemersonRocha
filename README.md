# Função para exibir o menu principal
def exibir_menu():
    print("Bem-vindo ao Programa de Introdução à Programação em Python")
    print("1. Tutorial")
    print("2. Exercícios Práticos")
    print("3. Projeto Simples")
    print("4. Sair")

# Função para executar o tutorial
def executar_tutorial():
    print("### Tutorial ###")
    print("Bem-vindo ao tutorial! Neste tutorial, vamos aprender um pouco sobre Python.")
    print("Python é uma linguagem de programação de alto nível e de sintaxe simples.")
    print("É amplamente utilizada em diversas áreas, como desenvolvimento web, ciência de dados e automação.")
    print("Em Python, você pode criar variáveis para armazenar dados. Os tipos de dados comuns incluem inteiros, flutuantes, strings e booleanos.")
    print("As estruturas de controle são ferramentas fundamentais na programação que permitem controlar o fluxo de execução de um programa. Elas permitem que você tome decisões com base em condições específicas e repita a execução de um bloco de código várias vezes. As principais estruturas de controle em Python são: (if, else, elif) e loops (for, while).")
    print("Essas estruturas de controle são essenciais para escrever programas que sejam capazes de tomar decisões dinâmicas e executar tarefas repetitivas de maneira eficiente. Elas fornecem a flexibilidade necessária para lidar com uma variedade de situações e automatizar tarefas comuns.")
    print("Entender esses conceitos básicos é um ótimo ponto de partida para aprender Python. À medida que você avança, pode explorar conceitos mais avançados, como orientação a objetos, manipulação de arquivos, tratamento de exceções e muito mais. A prática regular e a resolução de problemas reais são fundamentais para aprofundar seu conhecimento em Python.")

# Função para executar os exercícios práticos
def executar_exercicios():
    print("### Exercícios Práticos ###")
    print("EXERCÍCIO: Soma de Dois Números")
    num1 = int(input("Digite o primeiro número: "))
    num2 = int(input("Digite o segundo número: "))
    resultado = num1 + num2
    print("Resultado da soma:", resultado)
    print("EXERCÍCIO: Multiplicação de Dois Números")
    num1 = int(input("Digite o primeiro número: "))
    num2 = int(input("Digite o segundo número: "))
    resultado = num1 * num2
    print("Resultado da multiplicação:", resultado)
    print("3. Escreva um programa para imprimir os números primos até um determinado limite.")

# Função para executar o projeto simples
def executar_projeto():
    print("### Projeto Simples ###")
    print("Projeto: Calculadora Simples")
    print("Esta é uma calculadora simples em Python.")
    while True:
        print("\nOperações disponíveis:")
        print("1. Adição")
        print("2. Subtração")
        print("3. Multiplicação")
        print("4. Divisão")
        print("5. Sair")
        escolha = int(input("Escolha uma operação (1/2/3/4/5): "))
        if escolha == 5:
            break
        num1 = float(input("Digite o primeiro número: "))
        num2 = float(input("Digite o segundo número: "))
        if escolha == 1:
            resultado = num1 + num2
            print("Resultado da adição:", resultado)
        elif escolha == 2:
            resultado = num1 - num2
            print("Resultado da subtração:", resultado)
        elif escolha == 3:
            resultado = num1 * num2
            print("Resultado da multiplicação:", resultado)
        elif escolha == 4:
            if num2 == 0:
                print("Erro: divisão por zero!")
            else:
                resultado = num1 / num2
                print("Resultado da divisão:", resultado)
        else:
            print("Escolha inválida. Por favor, tente novamente.")


# Função principal
def main():
    while True:
        exibir_menu()
        opcao = input("Escolha uma opção: ")
        
        if opcao == "1":
            executar_tutorial()
        elif opcao == "2":
            executar_exercicios()
        elif opcao == "3":
            executar_projeto()
        elif opcao == "4":
            print("Obrigado por usar o Programa de Introdução à Programação em Python. Até logo!")
            break
        else:
            print("Opção inválida. Por favor, escolha uma opção válida.")

# Chamada da função principal
if __name__ == "__main__":
    main()
