# reto-bingo
# POR FAVOR LEA TODAS LAS INDICACIONES SUMINISTRADAS EN EL 
# ENUNCIADO ANTES DE EMPEZAR A IMPLEMENTAR SU SOLUCIÓN
from random import shuffle
# INSERTE SU IMPORTACIÓN
# from <LIBRERÍA> import <FUNCIÓN>

def balotera(balotas):
    # ACÁ INICIA LA FUNCIÓN
    B = I = N = G = O = False
    b = i = n = g = o = 0
    minimo_balotas = []
    shuffle(balotas)
    for balota in balotas:
        minimo_balotas.append(balota)
        if balota[0] == "B":
            b += 1
            if b == 5: B = True
        elif balota[0] == "I": 
            i += 1
            if i == 5: I = True
        elif balota[0] == "N": 
            n += 1
            if n == 4: N = True
        elif balota[0] == "G": 
            g += 1
            if g == 5: G = True
        elif balota[0] == "O": 
            o += 1
            if o == 5: O = True
        if (B and I and N and G and O): break
    balotas_revueltas = tuple(minimo_balotas)
    
  
    
    
    
    return balotas_revueltas
