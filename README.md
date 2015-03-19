# joguinho-1# -*- coding: utf-8 -*-
"""
Created on Thu Mar 19 12:33:00 2015

@author: carolinapiu
"""



p = 'pedra'
c = 'papel'
t = 'tesoura' 
s = 'spock'
l = 'lagarto'
from random import choice
com = ["pedra", "papel", "tesoura", "lagarto", "spock"]
computador = choice(com)
pcom = 0
ppe = 0
while pcom != 3 and ppe != 3:
    x = input("escolha pedra, papel, tesoura, spock ou lagarto")
    print (computador)
    if x == c:
        if computador == p or computador == s:
            print ("parabens, voce ganhou!")
            ppe += 1
            pcom = 0
        elif computador == x:
            print ("voce empatou")
            ppe = 0
            pcom = 0
        else:
            print ("voce perdeu")
            ppe = 0
            pcom += 1
    if x == p:
        if computador == l or computador == t:
            print ("parabens, voce ganhou!")
            ppe += 1
            pcom = 0
        elif computador == x:
            print ("voce empatou")
            ppe = 0
            pcom = 0
        else:
            print ("voce perdeu")
            ppe = 0
            pcom += 1
    if x == t:
        if computador == l or computador == c:
            print ("parabens, voce ganhou!")
            ppe += 1
            pcom = 0
        elif computador == x:
            print ("voce empatou")
            ppe = 0
            pcom = 0
        else:
            print ("voce perdeu")
            ppe = 0
            pcom += 1
    if x == l:
        if computador == s or computador == c:
            print ("parabens, voce ganhou!")
            pcom = 0
            ppe += 1
        elif computador == x:
            print ("voce empatou")
            pcom = 0
            ppe = 0
        else:
            print ("voce perdeu")
            pcom += 1
            ppe = 0
    if x == s:
        if computador == p or computador == t:
            print ("parabens, voce ganhou!")
            ppe += 1
            pcom = 0
        elif computador == x:
            print ("voce empatou")
            pcom = 0
            ppe = 0
        else:
            print ("voce perdeu")
            pcom += 1
            ppe = 0
if ppe == 3:
    print("parabens, voce ganhou o jogo!")
else:
    print("voce perdeu do computador")
   
        

