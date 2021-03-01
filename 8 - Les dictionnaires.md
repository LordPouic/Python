1 - Créer un dictionnaire stockant des personnes via leur nom (en clef) et leur age (en valeur)

```
PersonAge = {
    "Loic" : 30,
    "Christophe" : 5,
    "Marie" : 12,
    "Léa" : 65,
    "Julien" : 102,
    "Paul" : 2,
    "Joe" : 11,
    "Jen" : 58
}

```

2 - Créer une fonction permettant de connaitre le nom de la personne la plus vieille

```

def OldestPerson(Dict):
  KeyMax = None
  for key in Dict:
    if KeyMax == None:
      KeyMax = key
    elif Dict[key] > Dict[KeyMax]:
      KeyMax = key
  return KeyMax

print(OldestPerson(PersonAge))
```

3 - Créer une fonction permettant de connaitre le nombre de personnes majeures dans le le dictionnaire

```
def majeur(dic):
  c = 0
  for key in dic:
    if dic[key] >= 18:
      c = c + 1

  return c
```

4 - Créer le dictionnaire des résultats d'une compétition, chaque participant est défini par son numero d'inscrit,
trouver un moyen de stocker tous les résultats (en points) de chaque épreuves dans ce dictionnaire.

```

```

5 - Créer une fonction permettant de connaitre le vainqueur de la compétition (la personne ayant le plus de points)

```

```

6 - Créer une fonction qui prend en paramètre le numéro d'un inscrit et qui lui affiche la somme de ses points, ainsi que sa meilleure performance et sa pire.

```

```



