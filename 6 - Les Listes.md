1 - Créer une fonction créant une liste remplit de 50 fois la valeur 0

```
#L = [0,0,0,0,0,0,0,0,0,...]

def Liste50zero():
  L = []

  i = 0
  while i < 50:
    L.append(0)
    i = i + 1
  return L

LZ = Liste50zero()
print(LZ)
```

2 - Créer une fonction créant une liste de 20 cases chacune remplit par l’indice de la case 

```
#L = [0,1,2,3,4,5,6...]

def ListeIndice():
  L = []
  i = 0
  while i < 20:
    L.append(i)
    i = i + 1
  return L


Li = ListeIndice()
print(Li)
```

3 - Créer une fonction prenant un entier X en paramètre et créant une liste de X valeurs aléatoires 

```
from random import randint

def ListeAlea(X):
  L = []
  i = 0
  while i < X:
    L.append(randint(0,100))
    i = i + 1
  return L


print(ListeAlea(10))
```

4 - Créer une fonction calculant la moyenne des valeurs d'une liste remplit de chiffres

```
def Moyenne(Liste):
  S = 0
  i = 0
  while i < len(Liste):
    S = S + Liste[i]
    i = i + 1
  
  Moyenne = S / len(Liste)
  return Moyenne


L = ListeAlea(15)
print(L)
print(Moyenne(L))
```

5 - Créer une fonction créant 2 listes de valeurs aléatoires et qui donne en résultat une nouvelle liste qui est la concaténation des deux premieres

```
L1 = [1,2,3]
L2 = [5,4,3]
#1,2,3,5,4,3

L3 = L1 + L2
print(L3)
```

```
def ConcatListe(L1,L2):
  R = L1
  i = 0
  while i < len(L2):
    R.append(L2[i]) 
    i = i + 1
  return R

def ConcatListeFor(L1,L2):
  R = L1
  for x in L2:
    R.append(x) 
  return R

LX1 = ListeX(20)
LX2 = ListeX(5)
print(LX1)
print(LX2)
LX3 = ConcatListeFor(LX1,LX2)
print(LX3)
```

6 - Créer une fonction prenant une liste en entrée et la transformant pour lui enlever les valeurs 0

```
def Del0(Liste):
  i = 0
  while i < len(Liste):
    if Liste[i] == 0:
      Liste.remove(0)
    else:
      i = i + 1

  return Liste

def Del00(Liste):
  i = 0
  c = 0
  while i < len(Liste):
    if Liste[i] == 0:
      c = c + 1
    i = i + 1

  while c > 0:
    Liste.remove(0)
    c = c -1

  return Liste


def Del0For(Liste):
  c = 0
  for x in Liste:
    if x == 0:
      c = c + 1

  for i in range(c):
    Liste.remove(0)

  return Liste


T = [0,0,1,0,5,0,0]
T = Del0For(T)
print(T)
```

7 - Créer une fonction prenant une liste entrée et affichant la valeur maximale comprise dans cette liste

```
def Maximum(L):
  Max = L[0]
  i = 0
  while i < len(L):
    if L[i] > Max:
      Max = L[i]
    i = i + 1
  return Max

def MaximumFor(L):
  Max = L[0]
  for x in L:
    if x > Max:
      Max = x
  return Max

L = [1,2,4,6,85,7,9,2]
M = MaximumFor(L)
print(M)
```

8 - Créer une fonction prenant un entier et une liste en paramètre et qui affiche si oui ou non cet entier est présent dans cette liste

```
def Search(L,X):
  i = 0 
  while i < len(L):
    if L[i] == X:
      return True
    i = i + 1
  return False

def Searchfor(L,X):
  for v in L:
    if v == X:
      return True
  return False


Li = [0,1,2,5,4,8,75,3,2,4]
if Searchfor(Li,45) :
  print("La valeur est dedans")
else:
  print("Elle n'est pas là")
```

Bonus - Créer une fonction prenant en entrée une liste et affichant cette même liste mais triée par ordre croissant

```
Li = [1,3,4,5,6,8,7]

def TriBulle(L):
  j = 0
  while j < len(L):
    i = 0
    while i < len(L)-1:
      if L[i] > L[i+1]:
        T = L[i]
        L[i] = L[i+1]
        L[i+1] = T
      i = i + 1
    j = j + 1
  return L

Li = TriBulle(Li)
print(Li)
#Compléxité N²
```
```
L = [1,5,4,2,9,86,5,2,1,4,52,1]

def TriRapide(L):
  Pivot = L[len(L)/2]
  i = 0 
  Petit = []
  Grand = []
  while i < len(L):
    if L[i] < Pivot:
      Petit.append(L[i])
    else:
      Grand.append(L[i])
    i = i + 1



# complexité de NLog(N)
```



