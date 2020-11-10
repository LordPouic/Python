1 - Faire un programme qui prend l'age d'une personne et qui affiche si cette personne est majeure ou non.

```
Age = int(input())

if Age <0 or Age > 150:
  print("Error")
elif Age < 18:
  print("Mineur")
else :
  print("Majeur")
```

2 - Faire un programme qui prend deux valeurs et qui affiche la plus petite des deux

```
A = int(input())
B = int(input())

if A < B:
  print(A)
else:
  print(B)
```

3 - Même exercice que le 2 mais cette fois le programme prend 3 valeurs

```
A = int(input())
B = int(input())
C = int(input())

if A < B and A < C:
  print(A)
elif B < C:
  print(B)
else :
  print(C)
```

4 - Faire un programme qui prend une note au bac et qui affiche la mention assignée à cette note

```
Note = float(input())

if Note < 0 or Note > 20:
  print("Error")
elif Note < 10:
  print("Loupé")
elif Note < 12:
  print("Passable")
elif Note < 14:
  print("Assez bien")
elif Note < 16:
  print("Bien")
elif Note < 18:
  print("très bien")
else:
  print("Exellent")
```

5 - Faire un programme qui prend un chiffre et qui affiche si ce chiffre est pair ou impair

```
P = int(input())

if P%2 == 0:
  print("Pair")
else : 
  print("Impair")
```

6 - Ecrire un programme qui détecte si une année est bissextile

```
Annee = int(input())

# 8 -> Bissextile
# 200 - > Pas bissextile
# 800 - > Bissextile

if (Annee%4 == 0 and Annee%100 != 0) or Annee%400 == 0 :
  print("Bissextile")
else:
  print("Pas Bissextile")
```

