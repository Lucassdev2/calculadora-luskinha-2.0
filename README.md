# introdução a calculadora

print("═════════════════════""═════════════════════ \n")
print("CALCULADORA LUSKINHA 2.0 :")
print("═════════════════════""═════════════════════ \n")
print("O que veio com a atualização?")
print("•correcoes de bugs")
print("•ajustes no sistema de login")
print("•toda vez que você digitar /dados aparece as informações da conta : senha,idade,nome")
print("•texto")
print("•texto \n")

# sistema de login 2.0 (nome, idade, senha)
#usei o chat gpt para corrigir o bug na quantidade de idade 
print("sistema de login 2.0 \n")


nome = input("digite seu nome de usuário: ")
while len(nome) >= 9:
    print("voce excedeu o numero de caracteres,tente novamente \n")
    nome = input("digite seu nome de usuário: ")

else:
   print("seu nome de usuário é", nome, "\n")
   
idade = int(input("digite sua idade: "))
while idade <= 17:
      print("não aceitamos menores de idade")
      exit()
      
senha = input("defina sua senha como usuario:")
print("sua senha não pode passar de 12 caracteres")

while len(senha) > 12:
   print("senha invalida por excesso de caracteres! \n \n")
   print("digite novamente:")
   senha = input("degute sua senha como usuario: \n")


print("todos dados correspondentes \n")
print("algumas informacoes : " "\n nome:", nome, "\n idade : ", idade, "\n senha : ", senha ,"\n cuidado ao compartilhar sua senha de usuário \n \n \n")

#calculadora geral
print("╔═════════════════════" "lusΣka" "═════════════════╗ \n \n")

print("escolha uma função apenas digitando um número sugerido! \n")

print("[1]soma \n")
 #soma dois valores X e y inteiros
print("[2]Subtracao \n")
 #subtrai um valor X de Y sendo ambos inteiro
print("[3]mutiplicacao \n")
 #multiplica um valor X por um Y sendo ambos inteiros
print("[4]divisao \n")
 #divide um valor X por um y sendo ambos inteiros
print("[5]potenciacao \n")
 #porencia o valor de um valor X por um Y
print("[6]fatorcao \n")
 #fatora um valor X sendo o índice por um radicado Y

print ("╚═════════════════════" "lusΣka" "═════════════════╝\n \n")

opcao = int(input("Digite o número da operação desejada: "))

print(" \n reverificando seu perfil!")
senha_teste = input("digite sua senha por favor: \n")
   
while senha_teste != senha:
    senha_teste = input("digite novamente!!")
    
while senha_teste == senha:
   print(" \n")
   break

if opcao == 1:
    x = int(input("Digite o primeiro valor: "))
    y = int(input("Digite o segundo valor: "))
    resultado = x + y
    print("Resultado: ", resultado)

elif opcao == 2:
    x = int(input("Digite o primeiro valor: "))
    y = int(input("Digite o segundo valor: "))
    resultado = x - y
    print("Resultado: ", resultado)

elif opcao == 3:
    x = int(input("Digite o primeiro valor: "))
    y = int(input("Digite o segundo valor: "))
    resultado = x * y
    print("Resultado: ", resultado)

elif opcao == 4:
    x = int(input("Digite o primeiro valor: "))
    y = int(input("Digite o segundo valor: "))
    if y != 0:
        resultado = x / y
        print("Resultado: ", resultado)
    else:
        print("Não é possível dividir por zero!")

elif opcao == 5:
    x = int(input("Digite o valor da base: "))
    y = int(input("Digite o valor do expoente: "))
    resultado = x ** y
    print("Resultado: ", resultado)

elif opcao == 6:
    x = int(input("Digite o valor a ser fatorado: "))
    resultado = 1
    for i in range(1, x+1):
        resultado *= i
    print("Resultado: ", resultado)

else:
    print("Opção inválida.")
    
