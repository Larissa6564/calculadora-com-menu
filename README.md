# calculadora-com-menu
def calculadora():
    while True:
        print("\n===== CALCULADORA =====")
        print("1: Soma")
        print("2: Subtração")
        print("3: Multiplicação")
        print("4: Divisão")
        print("0: Sair")

        opcao = input("Digite o número da operação: ")

        if opcao == "0":
            print("Calculadora encerrada!")
            break

        if opcao not in ["1", "2", "3", "4"]:
            print("Essa opção não existe")
            continue

        numero1 = float(input("Digite o primeiro valor: "))
        numero2 = float(input("Digite o segundo valor: "))

        if opcao == "1":
            resultado = numero1 + numero2
            print(f"Resultado: {resultado}")

        elif opcao == "2":
            resultado = numero1 - numero2
            print(f"Resultado: {resultado}")

        elif opcao == "3":
            resultado = numero1 * numero2
            print(f"Resultado: {resultado}")

        elif opcao == "4":
            if numero2 == 0:
                print("Não é possível dividir por zero!")
            else:
                resultado = numero1 / numero2
                print(f"Resultado: {resultado}")


calculadora()
