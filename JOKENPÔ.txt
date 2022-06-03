print("{:=^30}".format("JO-KEN-PO"))
from random import randint
from time import sleep
opcoes = ("Pedra", "Papel", "Tesoura")
sorteio = randint(0, 2)
print("""Suas opções são:
[0] - Pedra
[1] - Papel
[2] - Tesoura""")
player = int(input("Qual a sua jogada? "))
if player > 2:
    print("\033[4;35;40mJOGADA INVÁLIDA\033[m")
    exit()
print("Jo")
sleep(1)
print("Ken")
sleep(1)
print("Pô")
sleep(1)
print("-=" * 10)
print("O computador escolheu {}".format(opcoes[sorteio]))
print("Você jogou {}".format(opcoes[player]))
print("-=" * 10)

if sorteio == 0:
    if player == 0:
        print("\033[33mEmpatou\033[m")
    elif player == 1:
        print("\033[32mVocê Venceu\033[m")
    elif player == 2:
        print("\033[31mO Computador Venceu\033[m")

elif sorteio == 1:
    if player == 0:
        print("\033[31mO Computador Venceu\033[m")
    elif player == 1:
        print("\033[33mEmpatou\033[m")
    elif player == 2:
        print("\033[32mVocê Venceu\033[m")

elif sorteio == 2:
    if player == 0:
        print("\033[32mVocê Venceu\033[m")
    elif player == 1:
        print("\033[31mO Computador Venceu\033[m")
    elif player == 2:
        print("\033[33mEmpatou\033[m")