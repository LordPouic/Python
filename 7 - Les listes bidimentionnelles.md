1 - Créer une fonction retournant une liste de dix cases chacune contenant une autre liste de 10 cases
    remplit par la valeur de l’indice de la première liste plus celui de la deuxième

```
def IndiceBidi():
  L = []
  i = 0
  while i < 10:
    T = []
    j = 0
    while j < 10:
      T.append(i+j)
      j = j + 1
    L.append(T)
    i = i + 1
  return L

Li = IndiceBidi()
i = 0 
while i < 10:  
  print(Li[i])
  i = i +1
```

2 - Créer une fonction prenant en paramètres deux chiffres T1 et T2 et retournant une liste de taille T1 
    contenant dans chaque case une liste de taille T2 remplit de chiffres aléatoires

```
from random import randint
def ListeBiAlea(T1,T2):
  L = [] 
  i = 0
  while i < T1:
    T = []
    j = 0 
    while j < T2:
      T.append(randint(0,100))
      j = j + 1
    L.append(T)
    i = i + 1
  return L


def ListeBiAleaFor(T1,T2):
  L = []
  for i in range (0,T1,1):
    T = []
    for i in range(0,T2,1):
      T.append(randint(0,100))
    L.append(T)
  return L

print(ListeBiAleaFor(3,4))

```

3 - Créer une fonction qui prend en paramètre une liste bidimensionnelle et un chiffre,
La fonction renvoie en retour oui ou non en fonction de si le chiffre est présent ou pas dans la liste.
    

```
def SearchBi(L,X):
  i = 0 
  while i < len(L):
    j = 0 
    while j < len(L[i]):
      if L[i][j] == X:
        return True
      j = j + 1
    i = i + 1
  return False
    

LA = ListeBiAleaFor(5,5)
print(LA)
print(SearchBi(LA,1))

```

4 - Créer une fonction qui calcule la somme des valeurs de toutes les cases d’une liste bidimensionnelle

```
def Somme(L):
  S = 0
  i = 0
  while i < len(L):
    j = 0
    while j < len(L[i]):
      S = S + L[i][j]
      j = j + 1
    i = i + 1
  return S

def SommeFor(L):
  S = 0
  for liste in L:
    for valeur in liste:
      S = S + valeur
  return S

LA = ListeBiAleaFor(2,2)
print(LA)
print(SommeFor(LA))

```
