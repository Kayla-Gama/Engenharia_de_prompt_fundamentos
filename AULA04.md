CODIGO SIMPLES: 
<img width="603" height="93" alt="Captura de tela 2026-04-01 203500" src="https://github.com/user-attachments/assets/61697d6b-05e9-44bc-b384-fb52a5c2dce6" />

# Solicita dois números ao usuário
numero1 = float(input("Digite o primeiro número: "))
numero2 = float(input("Digite o segundo número: "))

# Faz a soma
soma = numero1 + numero2

# Mostra o resultado
print("O resultado da soma é:", soma)


CODIGO ESTRUTURADO:
<img width="623" height="156" alt="Captura de tela 2026-04-01 203427" src="https://github.com/user-attachments/assets/b39244a8-a256-4abe-b9c9-ff672cb02d49" />

def somar_numeros():
    """
    Função responsável por solicitar dois números ao usuário,
    realizar a soma e exibir o resultado.
    """

    try:
        # Entrada de dados
        numero1 = float(input("Digite o primeiro número: "))
        numero2 = float(input("Digite o segundo número: "))

        # Processamento
        resultado = numero1 + numero2

        # Saída de dados
        print(f"\nResultado da soma: {resultado}")

    except ValueError:
        print("\nErro: Por favor, digite apenas números válidos.")


def main():
    """
    Função principal do programa.
    """
    print("=== Calculadora de Soma ===\n")
    somar_numeros()


# Garante que o programa só será executado diretamente
if __name__ == "__main__":
    main()



CODIGO EM FORMATO YAML: <img width="294" height="63" alt="Captura de tela 2026-04-01 203729" src="https://github.com/user-attachments/assets/6cb1f850-4f36-4be7-adb5-75ffb839545d" />

programa:
  nome: "Calculadora de Soma"
  descricao: "Programa simples para somar dois números informados pelo usuário"

  funcoes:
    somar_numeros:
      descricao: "Solicita dois números, realiza a soma e exibe o resultado"
      passos:
        - "Solicitar o primeiro número"
        - "Solicitar o segundo número"
        - "Converter os valores para float"
        - "Somar os dois números"
        - "Exibir o resultado"
      tratamento_de_erros:
        tipo: "ValueError"
        mensagem: "Digite apenas números válidos"

    main:
      descricao: "Função principal do programa"
      passos:
        - "Exibir mensagem de boas-vindas"
        - "Chamar a função somar_numeros"

  execucao:
    condicao: "__name__ == '__main__'"
    acao: "Executar a função main"

<img width="827" height="154" alt="Captura de tela 2026-04-01 203813" src="https://github.com/user-attachments/assets/8136b6cb-cace-4d73-9e2b-1f9893a2e50f" />
