1 - Ecrire une fonction qui prend en paramètre un texte et l'affiche 10 fois.

```
def Text10 (Txt):
  i = 0
  while i < 10:
    print(Txt)
    i = i + 1

Text10("Coucou")
```

2 - Ecrire une fonction qui prend un chiffre en paramètre et qui affiche la table de multiplication de ce chiffre

```
def TableMult(X):
  i = 1
  while i <= 10:
    print(X,"x",i,"=",X*i)
    i = i + 1

TableMult(5)
TableMult(10)
TableMult(124)
```

3 - Ecrire une fonction qui prend un chiffre en paramètre et qui affiche "error" si le chiffre et négatif ou sa table de multiplication si il est positif

```
def TableMultError(x):
  if x < 0:
    print("error")
  else :
    TableMult(x)


TableMultError(10)
```

4 - Créer une fonction qui prenant en entrée deux paramètres A et B et retournant A puissance B

```
def Puissance(A,B):
  R = A**B
  return R
```


```
# 1*2*2*2*2*2
def Puissances(A,B):
  P = 1
  i = 0
  while i < B:
    P = P * A
    i = i + 1
  return P
```

5 - Créer une fonction qui répond oui ou non au fait que le paramètre donné soit un chiffre premier ou pas

```
def Premier(X):
  i = 2
  P = 0
  while i < X:
    if X%i == 0:
      P = 1
    i = i + 1
  return P

D = Premier(int(input()))
if D==0:
  print("Premier")
```

6 - Créer une fonction qui prend en paramètre un chiffre et qui affiche tout les chiffres premiers inférieur au paramètre

```
def PremiersUnderX(X):
  i = 0
  while i < X:
    if Premier(i) == 0:
      print(i)
    i = i + 1

PremiersUnderX(500)
```

7 - Ecrire une fonction simulant un lancé de dé à 6 faces

```
from random import *

def De():
  return randint(1,6)
```

8 - faire un jeu à base de lancé de dés, le but est de faire, avec 3 dés une combinaison de trois fois la même valeur.
Pour cela il est possible de relancer jusqu'à 3 fois certains dès si leurs valeurs ne nous conviennent pas.


```
def GameisWin(d1,d2,d3):
  if d1 == d2 and d1 == d3:
    return 1
  else :
    return 0

def AskPlayer(NbDe):
  print("Voulez vous relancer le dé",NbDe,"Y/n")
  choix = input()
  if choix == "Y":
    return 1
  else:
    return 0

def Jeu():
  D1 = De()
  D2 = De()
  D3 = De()
  print(D1,D2,D3)

  i = 0
  while i < 3 and GameisWin(D1,D2,D3)==0 :
    if AskPlayer(1)==1:
      D1 = De()
    print(D1,D2,D3)
    
    if AskPlayer(2)==1:
      D2 = De()
    print(D1,D2,D3)

    if AskPlayer(3)==1:
      D3 = De()
    print(D1,D2,D3)

    i = i + 1

  if GameisWin(D1,D2,D3) == 1:
    print("Gagné")
  else:
    print("Perdu")


Jeu()
```

Bonus - Ecrire une fonction qui prend un nombre compris entre 1 et 3999 et qui affiche son équivalent en chiffre romain. 

```

```

