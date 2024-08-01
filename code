import os

import random

  

palavras_secreta = ['sunshine', 'beach', 'summer', 'surf', 'waves', 'shore']

os.system('cls')

print('Iniciando...')

  

while True:

    palavra_secreta = random.choice(palavras_secreta)

    letra_certa = ''

    tentativas = 0

    ganhou = False

  

    while True:

        letra_digitada = input('Digite uma letra: ')

        tentativas += 1

  

        if len(letra_digitada) > 1:

            print('Digite apenas UMA letra')

            continue

  

        if not letra_digitada.isalpha():

            print('Digite apenas LETRAS')

            continue

  

        if letra_digitada in palavra_secreta and letra_digitada not in letra_certa:

            letra_certa += letra_digitada

  

        palavra_formada = ''

        for letra_secreta in palavra_secreta:

            if letra_secreta in letra_certa:

                palavra_formada += letra_secreta

  

            else:

                palavra_formada += '*'

        print('Palavra secreta: ', palavra_formada)

  

        if palavra_formada == palavra_secreta:

            ganhou = True

            os.system('cls')

            print('PARABÉNS!! VOCÊ ACERTOU!')

            print('Tentativas: ', tentativas)

            sair = input('Sair? [s/n] ').lower().startswith('s')

            if sair:

                os.system('cls')

                break

  

            else:

                # Resetar as variáveis para começar um novo jogo

                os.system('cls')

                print('Recomeçando...')

                palavra_secreta = random.choice(palavras_secreta)

                letra_certa = ''

                tentativas = 0

  

    break
