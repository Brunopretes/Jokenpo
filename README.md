# JokEnPo
Jogo desenvolvido com base nas aulas do curso em video

from random import randint
from time import sleep
itens = ('Pedra', 'Papel', 'Tesoura', 'opção inválida')
computador = randint(0, 2)
print(''' Suas opções:
[0] Pedra!
[1] Papel!
[2] Tesoura!''')
print('*'*15)
jogador = int(int(input('Qual sua jogada?')))
if jogador >= 3:
    print('Jogada inválida, tente novamente!')
print('*'*15)
sleep(1)
print('\033[1;35m JO\033[m')
sleep(1)
print('\033[1;31m KEM\033[m')
sleep(1)
print('\033[1;32m PÔ!!!\033[m')
sleep(1)
print('*'*15)
print('Você escolheu {}'.format(itens[jogador]))
print('O computador escolheu {}'.format(itens[computador]))
print('*'*15)
if computador == 0:
    if jogador == 0:
        print('\033[1;35m EMPATE\033[m!')
    elif jogador == 1:
        print('\033[1;32m Eu Ganhei!\033[m')
    elif jogador == 2:
        print('\033[1;31m O computador ganhou!\033[m')
    else:
        print('Jogada invália, tente outra vez!')
elif computador == 1:
    if jogador == 0:
        print('\033[1;31mO computador ganhou!\033[m')
    elif jogador == 1:
        print('\033[1;35m EMPATE!\033[m')
    elif jogador == 2:
        print('\033[1;32m Eu Ganhei!\033[m')
    else:
        print('Jogada inválida, tente outra vez!')
elif computador == 2:
    if jogador == 0:
        print('\033[1;32m Eu Ganhei!\033[m')
    elif jogador == 1:
        print('\033[1;31m Computador ganhou!\033[m')
    elif jogador == 2:
        print('\033[1;35m EMPATE!\033[m')
    else:
        print('Jogada inválida, tente outra vez!')
print('*'*15)
