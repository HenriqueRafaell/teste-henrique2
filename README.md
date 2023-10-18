# teste-henrique2
para poder estudar

CODIGO DO CP DE PYTHON PARA PODER ESTUDAR 
print("Seja bem vindo à Vinheria!")
ano = input("Diga seu ano de nascimento : ")
endereco = input("Diga seu endereco : ")
while not ano.isnumeric():
    print("Deve ser um número com 4 caracteres!")
    ano = input("Diga seu ano de nascimento : ")
ano = int(ano)
if 2023 - ano < 18:
    print("Isso é muito feio!!!")
else:
    vinho1 = 'tinto'
    vinho2 = 'suave'
    vinho3 = 'seco'
    preco1 = 30
    preco2 = 40
    preco3 = 50
    qtd1 = 0
    qtd2 = 0
    qtd3 = 0
    valor_total = 0
    while True:
        print(f"Temos as seguintes opcoes: {vinho1} por R${preco1},00,\n"
              f"{vinho2} por R${preco2},00,\n"
              f"{vinho3} por R${preco3},00,")
        opcao = input("Qual voce vai levar ? (sair para encerrar) ")
        while opcao != vinho1 and opcao != vinho2 and opcao != vinho3 and opcao != 'sair':
            print("Deve ser uma opcao cadastrada!")
            opcao = input("Qual voce vai levar ? (sair para encerrar) ")
        if opcao == 'sair':
            if valor_total>500:
                print("Frete Grátis!!!")
            else:
                frete = 50
                print(f"Frete de R${frete},00")
                valor_total += frete

            print(f"Obrigado por comprar aqui. Voce comprou {qtd1} do {vinho1}, "
                  f"{qtd2} do {vinho2} e {qtd3} do {vinho3} totalizando"
                  f" R${valor_total},00 a ser entregue em {endereco}.")
            break
        qtd = input(f"Quantas garrafas do vinho {opcao} você vai levar ? ")
        while not qtd.isnumeric():
            print("Tem que ser um número!")
            qtd = input(f"Quantas garrafas do vinho {opcao} você vai levar ? ")
        qtd = int(qtd)
        if opcao == vinho1:
            valor_total += qtd*preco1
            qtd1 += qtd
        elif opcao == vinho2:
            valor_total += qtd*preco2
            qtd2 += qtd
        elif opcao == vinho3:
            valor_total += qtd*preco3
            qtd3 += qtd


CODIGOS DA AULA DE HJ PYTHON 18/10/2023
'''
i = 0
for i in range(10): #Faça com que certos caracteres assumam um certo valor, ou seja predefina um limite de coisas
    print(i)

i = 0
while i < 10:
    print(i)
    i+=1    #Repita enquanto uma condição for verdadeira
    #Nunca alterar a variavel dentro do looping do for, pra nao dar erro no codigo
    #range = conjunto com os valores que minha variavel vai assumir
    #Len mede a quantidade de objetos no conjunto
#for e while ambos são estruturas de repetição
'''
'''
i = 0
for i in range(10):
    print(i)
print()
for char in 'danilo':
    print(char)
'''
'''
for i in range(1,100,7):
    print(i)

for i in range(0,100,2):
    print(i)

for i in range(0,10,-2):
    print(i) 
'''
'''
soma = 0
for i in range(5):
    nota = int(input("Diga sua nota : "))
    soma += nota
print(soma/5)
'''
'''
senha = '1234'
usuario = 'henrique'
for login in range(3):
    usuario = input("Diga seu usuario : ")
    senha = int(input("Diga sua senha : "))
    if usuario == usuario and senha == senha:
        print("Acesso liberado ")
        break
'''
'''
for num in range(1,11):
   print(f"\n Tabuada do {num} : ")
   for i in range(1,11):
      print(f"{num} * {i} = {num*i}", end=',')
'''
'''
lista = [0,2,1,'idsffh', True]
for elem in lista:
    print(elem)
'''
'''
lista = [30,40,50,60,70,80,90,]
for elem in lista:
    elem = 1
print(lista)


for i in range (len(lista)):
    lista[i] = i
print(lista)
'''
'''
lista = []
lista.append(34)
print(lista)
lista.append(50)
print(lista)
'''
'''
soma = 0
lista = []
nota = 5
for i in range(5):
    nota = int(input("Diga sua nota : "))
    lista.append(nota)
    soma+=nota
    print(lista)
print(soma/5)
if nota <= 5:
    print("Essa nota esta a baixo da média ")
if nota >= 6:
    print("Você está a cima da média!")
'''
'''
nomes = ['Danilo,Henrique,Rafael,Pedro,Jose,João,Maria,Thiago,Marcelo,Kevin']
for i in range(len(nomes)):
    if nomes[i] == "Danilo":
        print("O DANILO É TOP!!")
        print(f"Encontrei no indice {i}")
'''

lista = [4,2,6,7,5,1]
maior = lista[0]
for i in range(len(lista)):
    candidato = lista[i]
    print(f"Vou testar se o {candidato} > {maior}")
    if candidato > maior:
        print(f"Troquei o  {maior} por {candidato}")
        maior = candidato











