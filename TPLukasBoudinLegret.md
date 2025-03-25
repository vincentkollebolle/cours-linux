**Mini TP : Gestion d’une bibliothèque avec Linux**

**Objectif :** Acquérir une bonne compréhension des commandes Linux de base en les
appliquant à un scénario concret : la gestion d’une bibliothèque de livres numériques.

**Page 1 : Énoncé du TP**

**Instructions générales :**

```
 Pour chaque question, réfléchissez à la commande la plus adaptée et testez-
  la.
 Notez vos réponses dans un fichier reponses.txt en expliquant ce que fait
  chaque commande utilisée.
 Si vous bloquez, utilisez man ou --help pour trouver des indices.
```
**1. Création de la bibliothèque**
    1. Créez un dossier principal nommé Bibliotheque et entrez dedans.
    2. Comment pouvez-vous vérifier que vous êtes bien dans le bon dossier?
    3. Listez le contenu de votre répertoire. Que voyez-vous?

**2. Organisation des livres**
    1. Créez deux dossiers : Romans et Science_Fiction.
    2. Créez trois fichiers texte correspondant à des livres (livre1.txt, livre2.txt,
       livre3.txt).
    3. Déplacez livre1.txt dans Romans et copiez livre2.txt dans Science_Fiction.
    4. Affichez une liste détaillée des fichiers et dossiers présents dans Bibliotheque.

**3. Gestion du contenu des fichiers**
    1. Ajoutez du texte dans livre1.txt sans ouvrir d’éditeur de texte.
    2. Affichez le contenu de livre1.txt.
    3. Affichez uniquement les 5 dernières lignes de livre1.txt. Que remarquez-vous
      ? (la commande tail pourrait être utile)
    4. Utilisez une commande pour afficher progressivement le contenu de livre1.txt.

**4. Recherche et modification de contenu**
    1. Recherchez si le mot "histoire" est présent dans livre1.txt.
    2. Remplacez le mot "histoire" par "roman" dans livre1.txt.
    3. Vérifiez que la modification a bien été prise en compte.

**5. Gestion avancée**
    1. Affichez uniquement les fichiers .txt présents dans Bibliotheque et ses sous-dossiers.
    2. Redirigez la liste des fichiers de Bibliotheque vers un fichier contenu_bibliotheque.txt.
    3. Filtrez ce fichier pour n’afficher que les fichiers contenant "livre" dans leur nom.
    4. Comment pouvez-vous afficher la documentation d’une commande que vous ne connaissez pas bien?

**6. Nettoyage et téléchargement**
    1. Nettoyez l’affichage du terminal.
    2. Téléchargez un livre en ligne au format texte et placez-le dans Bibliotheque sous le nom Orgue_et_Prejuges.txt. (https://www.gutenberg.org propose des ebooks gratuits et wget pourrait nous être utile)

**Page 2 : Correction du TP**

**1. Création de la bibliothèque**

```
1 mkdir Bibliotheque crée le dossier.
2 cd Bibliotheque permet d’y entrer.
3 pwd affiche le chemin du dossier actuel.
4 ls permet de voir son contenu.
```
**2. Organisation des fichiers**

```
1 mkdir Romans Science_Fiction crée les dossiers.
2 touch livre1.txt livre2.txt livre3.txt crée trois fichiers.
3 mv livre1.txt Romans/ déplace livre1.txt.
4 cp livre2.txt Science_Fiction/ copie livre2.txt.
5 ls -l affiche les fichiers en détail.
```
**3. Gestion du contenu des fichiers**

```
1 echo "Ceci est un roman passionnant." > Romans/livre1.txt ajoute du texte.
2 cat Romans/livre1.txt affiche le contenu.
3 tail - n 5 Romans/livre1.txt montre les 5 dernières lignes.
4 less Romans/livre1.txt permet un affichage paginé.
```
**4. Recherche et modification de contenu**

```
1 grep "histoire" Romans/livre1.txt cherche le mot "histoire".
2 sed -i 's/histoire/roman/' Romans/livre1.txt remplace "histoire" par "roman".
3 cat Romans/livre1.txt permet de vérifier la modification
```
**5. Gestion avancée**

```
1 find. -name "*.txt" liste tous les fichiers .txt.
2 ls -R > contenu_bibliotheque.txt stocke la liste des fichiers dans un fichier.
3 grep "livre" contenu_bibliotheque.txt filtre les fichiers contenant "livre".
4 man grep affiche la documentation de grep.
```
**6. Nettoyage et téléchargement**

```
1 clear nettoie l'affichage du terminal.
2 wget https://www.gutenberg.org/cache/epub/1342/pg1342.txt -O Orgue_et_Prejuges.txt télécharge le livre.
```


