# Sorteio-de-Nomes-e-Cores-Listas-diferentes-com-Python
https://medium.com/@p.joycii/sorteio-de-nomes-e-cores-listas-diferentes-com-python-9fa3b295f223

import random


participantes_sorteio = ["Maro", "Joyci", "Grazi", "Fábio", "Larissa", "Diego"]
cores = ["Azul", "Verde", "Preto", "Rosa", "Vermelho", "Amarelo"]

print('********* ESCOLHENDO CORES *************')

i=len(participantes_sorteio)


while i > 0:
    escolha_nome = random.choice(participantes_sorteio)
    novo_sorteio_nome = participantes_sorteio.remove(escolha_nome)

    escolha_cor = random.choice(cores)
    novo_sorteio_cor = cores.remove(escolha_cor)
    i = i-1

    print('Para '+ escolha_nome +' a cor sorteada foi: ' + escolha_cor)
