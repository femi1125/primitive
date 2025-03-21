# primitive
Algorithme primitive
Variable
  n, i : entier
 coeff[n], prim[n+1]: tableau d'entiers   
DEBUT
    ECRIRE: ("Entrez le degré du polynôme : ")
    LIRE: n
     POUR i = 0 JUSQU'À n FAIRE
        ECRIRE "Entrez le coefficient du monôme de degré", i, " : "
        LIRE coeff[i]
     FIN POUR
     POUR i = 0 JUSQU'À n FAIRE
        prim[i+1] ← coeff[i] / (i + 1)
     FIN POUR
    ECRIRE "La primitive de f(x) est : "
      POUR i ← 1 JUSQU'À n+1 FAIRE
        SI i = 1 ALORS
            ECRIRE prim[i], "x^", i
        SINON
            ECRIRE " + ", prim[i], "x^", i
        FIN SI
     FIN POUR
  ECRIRE " + C"  
FIN
