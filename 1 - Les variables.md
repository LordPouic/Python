
1 - Ecrire un programme ayant une variable C, donner une valeur à C, calculer et afficher son carré

```
C = float(input())
C = C * C
print(C)
```

2 - Ecrire un programme ayant deux variable A et B, donner des valeurs à A et B puis tenter de trouver un moyen d’intervertir les deux valeurs contenues dans A et B

```
A = 2
B = 3
print(A,B)
C = A
A = B
B = C
print(A,B)
```

```
A = 2
B = 3
print(A,B)
A,B = B,A
print(A,B)
```

```
A = 2
B = 3
print(A,B)

A = A + B
B = A - B
A = A - B

print(A,B)
```

```
A = 2
B = 3
print(A,B)

A = A ^ B
B = A ^ B
A = A ^ B

print(A,B)
```

3 - Ecrire un programme ayant une variable R correspondant au rayon d’un cercle, donner une valeur à R et calculer le périmètre du cercle de rayon R

```
from math import pi

Rayon = float(input())
Peri = 2 * Rayon * pi
print(Peri)
```

4 - Ecrire un programme ayant 4 variables correspondant à 4 notes, donner des valeurs aux variables et écrire un algorithme permettant de calculer la moyenne de ces 4 notes

```
N1 = float(input())
N2 = float(input())
N3 = float(input())
N4 = float(input())

Moyenne = (N1 + N2 + N3 + N4)/4
print(Moyenne)
```

5 - Ecrire un programme ayant une variable S contenant des secondes. Afficher le nombre d'heures et de minutes correspondantes.


```
Sec = 10000
H = Sec//3600
Sec = Sec % 3600
Min = Sec//60
Sec = Sec % 60

print(H,"h", Min,"min", Sec,"Sec")
```
