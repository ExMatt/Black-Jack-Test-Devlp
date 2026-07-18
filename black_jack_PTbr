#Apresentação
print("----------------")
print("-Bem Vindo a 21-")
print("----------------")

print("\n--------")
print("-Regras-")
print("--------")

print("1 - No inicio da rodada de cada jogador, esse escolherá se deseja ou não receber de 1 a 10 pontos\n")
print("2 - Caso qualquer jogador ultrapasse o limite de 21 pontos, o mesmo perde imediatamente")
print("4 - O jogador mais proximo de 21 pontos vence")
print("3 - Caso os jogadores tirem o mesmo número, o resultado é empate\n")

#Inicio
from random import randint

P1 = 0
P2 = 0

P1f = False
P2f = False

RespostaS = ["s","sim"]
RespostaN = ["n","nao"]

while True:
        
    
    if P1f == False:
        Resposta1 = input("Jogador \033[1m1\033[0m, Gostária de receber os pontos?: ")
        if Resposta1.lower() in RespostaN:
            print(f"\nJogador \033[1m1\033[0m Encerrou a Rodada com \033[1m{P1}\033[0m Pontos!")
            P1f = True
            pass
        elif Resposta1.lower() in RespostaS and P1 <= 21:
            Luck = randint(1,10)
            P1 += Luck
            print(f"\nJogador \033[1m1\033[0m Recebeu \033[1m{Luck}\033[0m Pontos!")
            print(f"\nJogador \033[1m1\033[0m Possui \033[1m{P1}\033[0m Pontos!")
            if P1 > 21:
                print("\nJogador \033[1m1\033[0m \033[1mQuebrou\033[0m o limite de pontos!")
                P1f = True
        else:
            print("\nInsira um valor válido. Sim ou Nao.")
            continue
    else:
        pass

    if P2f == False:
        Resposta2 = input("\nJogador \033[1m2\033[0m, Gostária de receber os pontos?: ")
        if Resposta2.lower() in RespostaN:
            print(f"\nJogador \033[1m2\033[0m Encerrou a Rodada com \033[1m{P2}\033[0m Pontos!")
            P2f = True
            pass
        elif Resposta2.lower() in RespostaS and P2 <= 21:
            Luck = randint(1,10)
            P2 += Luck
            print(f"\nJogador \033[1m2\033[0m Recebeu \033[1m{Luck}\033[0m Pontos!")
            print(f"\nJogador \033[1m2\033[0m Possui \033[1m{P2}\033[0m Pontos!\n")
            if P2 > 21:
                print("\nJogador \033[1m2\033[0m \033[1mQuebrou\033[0m o limite de pontos!\n")
                P2f = True
        else:
            print("\nInsira um valor válido. Sim ou Nao.")
            continue
    else:
        pass
    
    if P1f and P2f == True:
        break

if P1f > P2f and P1f <= 21:
    print("------------------")
    print("-Jogador 1 Venceu-")
    print("------------------")
elif P1f == P2f:
    print("-------------------------")
    print("-Os Jogadores empataram!-")
    print("-------------------------")
else:
    print("------------------")
    print("-Jogador 2 Venceu-")
    print("------------------")