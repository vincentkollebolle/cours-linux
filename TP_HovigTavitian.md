# Exercice :

### 1. Créez un dossier `exercice_linux` et entrez dedans.

### 2. Créez trois fichiers : `fichier1.txt`, `fichier2.txt`, `fichier3.txt`.

### 3. Listez le contenu du dossier.

### 4. Ajoutez du texte dans `fichier1.txt`.

### 5. Copiez `fichier1.txt` dans un dossier `dossier1`.

### 6. Déplacez `fichier2.txt` dans `dossier1`.

### 7. Listez le contenu de `dossier1`.

### 8. Affichez le contenu de `fichier1.txt`.

### 9. Ajoutez une deuxième ligne à `fichier1.txt`.

### 10. Affichez les 2 premières lignes de `fichier1.txt`.

### 11. Affichez la dernière ligne du fichier.

### 12. Recherchez le mot "fichier" dans `fichier1.txt`.

### 13. Remplacez "fichier" par "document" dans `fichier1.txt`.

### 14. Affichez uniquement le premier mot de chaque ligne.

### 15. Effacez l’écran du terminal.

### 16. Téléchargez la page d’accueil de Wikipedia.

### 17. Affichez les premières lignes du fichier téléchargé.

### 18. Affichez le manuel de la commande `grep`.

# Corigé :

## 1.
```bash
mkdir exercice_linux
cd exercice_linux
```

## 2.
```bash
touch fichier1.txt fichier2.txt fichier3.txt
```

## 3.
```bash
ls
```

## 4.
```bash
echo "Ceci est le fichier numéro 1" > fichier1.txt
```

## 5.
```bash
mkdir dossier1
cp fichier1.txt dossier1/
```

## 6.
```bash
mv fichier2.txt dossier1/
```

## 7.
```bash
ls dossier1
```

## 8.
```bash
cat fichier1.txt
```

## 9.
```bash
echo "Deuxième ligne du fichier 1" >> fichier1.txt
```

## 10.
```bash
head -n 2 fichier1.txt
```

## 11.
```bash
tail -n 1 fichier1.txt
```

## 12.
```bash
grep "fichier" fichier1.txt
```

## 13.
```bash
sed -i 's/fichier/document/g' fichier1.txt
```

## 14.
```bash
awk '{print $1}' fichier1.txt
```

## 15.
```bash
clear
```

## 16.
```bash
wget https://www.wikipedia.org
```

## 17.
```bash
head -n 10 index.html
```

## 18.
```bash
man grep
```


