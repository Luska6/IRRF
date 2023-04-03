# IRRF
//Calculo do IRRF BR

seusal = float(input('QUAL O VALOR DO SEU SALARIO?'))
print(seusal)
if seusal <= 1751.81:
    aliq=0.08
if seusal >= 1751.82 and seusal <= 2919.72:
    aliq=0.09
if seusal >= 2919.73:
    aliq=0.11 
if seusal >= 5839.45:
    inss = 5839.45*0.11
else:
    inss = seusal*aliq
print (inss)
mlk = int (input('QUAL O NUMERO DE DEPENDENTES?'))
print(mlk)
desc1 = mlk*189.59
print (desc1)
pensao = float (input('QUAL O VALOR DA PENSAO?'))
desc2 = pensao
print (desc2)
privada = float (input('VALOR PAGO DA PREVIDENCIA PRIVADA PAGO'))
desc3 = privada
print (desc3)
FINALLE = float (seusal-inss-desc1-desc2-desc3)
print (FINALLE)
if FINALLE <= 1903.98:
    aliq2=0
if FINALLE >= 1903.99 and FINALLE <= 2826.65:
    aliq2=0.075 
    DEDUZ = 142.80
if FINALLE >= 2826.66 and FINALLE <= 3751.05:
    aliq2=0.15
    DEDUZ = 354.8
if FINALLE >= 3751.06 and FINALLE <= 4664.68:
    aliq2=0.225
    DEDUZ=636.13
if FINALLE >= 4664.68:
    aliq2=0.275
    DEDUZ=869.36
print (FINALLE)
VALORIR =FINALLE*aliq2
VALORIR1 = VALORIR - DEDUZ
print (VALORIR1)
saliq = float (seusal-inss-desc1-desc2-desc3-VALORIR)
print (saliq)
input ('')
