# Notes introduction au python
## Python course to make bio students understand a bit of python

## Table of matters
1. [Les variables](#Les-variables)  
   a) [Notation](#Notation)  
   b) [Visibilité des variables](#Visibilité-des-variables)  
3. [Les fonctions](#Les-fonctions)  
   a) [Les fonctions "manuelles"](#Les-fonctions-"manuelles")  
   b) [Les fonctions intégrées](#Les-fonctions-intégrées)  
4. [Les types](#Les-types)
5. [Les opérateurs](#Les-opérateurs)
6. [Dictionnaire et liste](#Dictionnaire-et-liste)  
   a) [Dictionnaire](#Les-fonctions-"manuelles")  
   b) [Liste](#Les-fonctions-intégrées)  
7. [Les comapratifs](#Les-comparatifs)  
   a) [IF/ELSE](#IF/ELSE)  
   b) [WHILE](#WHILE)  
   c) [FOR](#FOR)  
8. [Exos](#Exos)
9. [TL;DR](#TL-DR)

### Les variables

#### Notation

On note tout en minuscule séparé par des underscores + le premier caractère n’est pas un nombre. Aussi, on utilise pas d’accents  

```ma_var1 = 1```  

#### Visibilité des variables
En ayant compris que l’indentation en python permet de rentrer dans des “blocs de code” (if, else, while, for (représentés par : à la fin de ces lignes)), nous pouvons comprendre le principe de visibilité des varibales. 

Comme pour la théorie des ensembles, la visibilité des variables consiste en la déclaration des variables au bon endroit du code. 

Déclarer ses variables à la première indentation du code et au début du fichier ménera à la limitation d’erreurs. 

En effet, l’interpréteur python exécute le programme de bas en haut. 

Il faut donc qu’il connaisse les éléments qu’on lui donne. 

Tu peux me parler de ton ami sans me l’avoir présenté. Si tu me nommes ton ami avant je comprends ton histoire. 

### Les fonctions 

#### Les fonctions “manuelles” 

Généralement, les fonctions sont des “processus” qui peuvent prendre des entrées 	et créer des sorties. Elles peuvent être appelées pour être réutilisées.  
```
def ma_fonction1(age, taille):
    print(“Vous avez “ + age + “ an(s) et mesurez “ + taille “ cm.”)
    return age
ma_fonction1(20, 172)
```
Le programme affichera :
```
Vous avez 20 an(s) et mesurez 172 cm.
```
Ma_fonction1 est ici égale à 20 car on retourne “age”.

#### Fonctions intégrées 

```len(a)``` -> donne le nombre d’éléments de a -> len pour lenght = longueur 

```var.append(élément_à_ajouter)``` -> ajouter à une liste []. Se note var_stock_list.append(élément) 

```round(x)``` -> arrondi le float x 

```int(var)``` -> “transforme” une valeur non int en integer 

```str(var)``` -> “transforme” une valeur non str en string 

```float(var)``` -> “transforme” une valeur non float en float 

### Les types 

```int```, ```float```  -->  chiffres 

```string```  -->  lettres 

```bool```  -->  booléens correspondants à True ou False (majuscule importante ici) 

Dict, list, tableau  -->  stockage de donnée {key, valeur} [1, 2]  

### Les opérateurs

```+```, ```-```, ```*```, ```/```, ```**```, ```%```  
Explicite sinon ** correspond aux puissances et % au résultat de la division euclidienne 		(nommée “modulo”) 

### Dictionnaire et liste

#### Dictionnaire 

```my_dict = {}```

Add something to a dict with key = email and value = alice@example.com 

```my_dict["email"] = "alice@example.com"```  
```print(my_dict["email"])```  
Returns "alice@example.com"

#### Liste 

```tortue = []```
```print(tortue)``` retourne rien  
```tortue.append(“élément”)``` Tortue contient maintenant l’élément “élément”. 
```print(tortue)``` retourne éléments de la liste

On peut récupérer les éléments des listes avec leur postion allant de 0 jusqu’au nombre d’élément dans la liste –1 (du coup vu qu’on commance de 0) 

Pour récupérer la suite d’élements avec le premier compris et le dernier exclu, par exemple, on a : 

```ma_list = [1, 2, 3, 4, 5]```  
```print(ma_list[1:5])```  
Retourne [2, 3, 4, 5] -> 2 étant à la position 1 et 5 le max car il n'y a que 4 positions (0 à 4 = 5)  
Ma_list[4] retourne 5 qui est en postition 4 (de 0 à 4 toujours)  

Pour lister le nombre d’éléments d’une liste on a :  
```Print(Len(ma_list))```  
5, il y a en effet bien 5 éléments dans cette liste 

### Les comparatifs 
Voici une liste de comparatifs (optionnel) 
```mes_comparatifs = [==, !=, <, >, <=, >=]```   
Les mots clés ```and```, ```or``` et ```not``` fonctionnent pour vérifier deux conditions à la fois par example	 

#### IF/ELSE 

```
nombre = 2 

  if nombre == 1:			 

      print(“patate”) 

  else: 

      print(“famine”)
```

#### WHILE 

```
Nombre=200 

While nombre!=1: 

      nombre= nombre –1 

If nombre = 1: 

      Print(“patate”)
```

#### FOR 
```
for i in range(10) 
    print(i) 
```

### Exos 

#### Exo IMC  
```
taille = input(“Quel est votre taille ?”) 
taille = Int(taille) 
poids= input(“Quel est votre poids?”) 
poids = int(poids) 
IMC = poids/taille**2 
print(IMC)
``` 

### TL DR 

```Ma_variable1 = “bonjour”```  

```
def ma_fonction(paramètre_de_fonction, deuxième_paramètre_de_fonction): 
    return résultat
```  

```
if condition == constante: 
    exécution 
else: 
    autre exé
```  

```
while condition: 
    exécution
Ici, à la fin de l’exé faire qqch
```

```
for a in range(6, 8):
    print(i)
```   

```Print()```  -->  affiche (texte ou variable) 

```Input(“question à l’utilsateur”)```  -->  demande quelque chose à l'utilsateur

Fonctions intégrées : ```Int()``` / ```float()``` / ```str()```  
```var.Append(élément)``` / ```len(var)``` / ```round(var)``` 

Types : ```Int``` / ```float``` / ```str``` / ```bool```  

Stockage : ```dict {key: value}``` / ```list []``` / tableau   

Comparatifs : ```==``` / ```!=``` / ```<``` / ```>``` / ```<=``` / ```>=```  

Opérateur pour 1 ou 2 : ```and``` / ```or``` / ```not``` 

	 
