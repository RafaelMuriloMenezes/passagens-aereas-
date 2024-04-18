# passagens-aereas-
Passagem aéreas - Projeto Python 
from menu import  mostrar_menu  
from passagens import Passagem, PassagensAereasManager                   
#Fim da Função
    
while True:
    passagens_areas_manager = PassagensAereasManager()
    Valor = int(input())

    if Valor == 1: 
        print ('Você escolheu opção 1')
        origem = input ( "Qual é a origem?")    
        destino = input ("Qual o destino?")  
        preco = input ("Qual o preco?")

        passagem = Passagem(origem, destino, preco)
        passagens_areas_manager.adicionar_passagem(Passagem)

    elif Valor == 2: 
        print('Você escolheu opção 2')
        print(passagens_areas_manager.passagenscomprada)

    elif Valor == 3:
        print('Você encerrou o programa, volte novamente!')
        break
