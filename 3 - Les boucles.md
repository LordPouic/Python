1 - Via une boucle afficher tous les chiffres entiers de 100 à 1

```
C = 100
while C > 1:
  print(C)
  C = C - 1
```

2 - Via une boucle afficher tous les chiffres pairs de 1 à 100

```
C = 0
while C < 100 :
  if C%2 == 0:
    print(C)
  C = C + 1
```


3 - Via une boucle écrire un programme qui calcule la somme des 10 premiers chiffres entiers

```
A = 0
S = 0

while A < 10:
  S = S + A
  A = A + 1

print(S)
```

4 - Faire un programme qui prend 10 notes aléatoires et affiche affiche la moyenne des notes

```
from random import *

C = 0
Somme = 0

while C < 500 :
  Somme = Somme + randint(0,20)
  C = C + 1

Moyenne = Somme / 500
print(Moyenne)
```

5 - Ecrire un programme qui prend un chiffre et qui affiche sa table de multiplication.

```
Chiffre = int(input())
i = 0
while i <10:
  i = i + 1
  r = Chiffre * i
  print(Chiffre,"*",i,"=",r)
```

6 - Ecrire un programme qui prend un nombre et calcule la factorielle de ce nombre.

```
i = 1
fact = int(input())
result = 1

while i <= fact:
  result = result * i
  i = i + 1

print(result)
```

7 - Ecrire un programme ayant une variable dont la valeur est à deviner, le programme va demander en boucle une réponse et afficher soit trop haut ou trop bas tant que 
la valeur rentrée n'est pas la bonne.

```
from random import *
ChiffreSecret = randint(0,1000)
Proposition = int(input())

while Proposition != ChiffreSecret:
  if Proposition > ChiffreSecret:
    print("Trop haut")
  else :
    print("Trop bas")

  Proposition = int(input())

print("Winner")
```

Bonus - Ecrire un programme qui calcule la 20eme valeur de la suite de Fibonacci.

```
V1 = 1 
V2 = 1

Limite = int(input())

i = 0
while i < limite:
  V3 = V1 + V2
  V1 = V2
  V2 = V3
  i = i + 1 
  print(V3)
```

Bonus - Ecrire un programme détectant les nombres de Armstrong compris entre 0 et 999.

```
i = 0
while i < 1000:
  U = i%10
  D = (i//10)%10
  C = i//100
  if i == U*U*U + D*D*D + C*C*C:
    print(i)
  
  i = i + 1
```

----Exercices complémentaires----

Ecrire un programme qui prend un chiffre donné par l'utilisateur (positif ou négatif) et qui affiche tous les nombres compris entre ce nombre et zero

```
Chiffre = int(input())

if Chiffre >=0: 
  i = 0
  while i<Chiffre:
    print(i)
    i = i + 1
else:
  i = 0
  while i>Chiffre:
    print(i)
    i = i - 1
```

Ecrire un algorithme prenant un nombre entier donné par l'utilisateur et qui l'affiche à l'envers (12345 devient 54321)

```
C = 15542864
R = ""

while C > 0:
  dernierChiffre = C%10
  R = R + str(dernierChiffre)
  C = C//10

print(R)
```

Ecrire un algorithme qui demande 10 valeurs à un utilisateur et qui affiche à la fin le plus petit nombre donné

```
i = 0 
min = int(input())

while i<9:
  V = int(input())
  if V < min:
    min = V
  i = i + 1

print(min)
```
Trouver un moyen d'écrire un programme prenant un chiffre et affichant une figure comme celle ci (pour un chiffre entré de 9) :<br>
0000000000<br>
111111111<br>
22222222<br>
3333333<br>
444444<br>
55555<br>
6666<br>
777<br>
88<br>
9<br>

```
C = int(input())
i=0
while i < C:
  print( str(i) * (C-i))
  i = i + 1

```

