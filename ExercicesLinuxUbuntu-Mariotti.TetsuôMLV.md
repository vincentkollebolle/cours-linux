**<u>Feuille envoyer Alexis Barbier.</u>**

**<u>Exercices Non Corriger A FAIRE :</u>**

<u>Exercice1:Explorer unrépertoireavec ls.</u>

**<u>Consignes :</u>**

1\. Affichez la liste de

2.Affichez la liste des fichiers et dossiers dans votre répertoire
personnel. 3.Affichez la liste des fichiers avec leurs détails
(permissions, taille, propriétaire, etc.).

4.Affichez uniquement les fichiers cachés. 5.Affichez les fichiers triés
par taille.

6.Affichez la liste des fichiers avec leurs tailles au format lisible
(K, M, G).

<u>Exercice 2 : Créer des fichiers et des dossiers avec mkdir et
touch.</u>

**<u>Consignes :</u>**

1.Créez un répertoire nommé projet dans votre dossier personnel.
2.Accédez à ce répertoire.

3.Dans projet, crée trois sous-dossiers : docs, scripts, logs. 4.Dans le
dossier docs, créez un fichier nommé README.txt. 5.Dans le dossier
scripts, créez un fichier install.sh.

**<u>Exercice 3 : Créer un utilisateur et gérer ses droits</u>**

**<u>Consignes :</u>**

1.Créez un nouvel utilisateur nommé devuser. 2.Définissez un mot de
passe pour devuser. 3.Vérifiez que l'utilisateur a bien été créé.

4.Accordez-lui les droits de lecture et d'écriture sur le dossier
projet.

**<u>Exercice 4 : Déplacer un fichier dans le dossier de
l'utilisateur</u>**

**<u>Consignes :</u>**

1.Déplacez le fichier install.sh créé dans **Exercice** **2** vers le
dossier personnel de devuser.

2.Vérifiez que le fichier a bien été déplacé.

3.Changez le propriétaire du fichier pour que devuser en ait le
contrôle.

**<u>Exercice 5 : Rechercher du texte avec grep</u>**

**<u>Consignes :</u>**

1.Créez un fichier texte logfile.txt et ajoutez-y les lignes suivantes :
(Tu peux utiliser nano, vim, ou echo pour créer et éditer le fichier.)
2.Affichez toutes les lignes contenant le mot Erreur.

3.Affichez toutes les lignes contenant Succès, en ignorant la casse
(Succès/ succès).

4.Comptez le nombre de lignes contenant le mot Info.

5.Recherchez uniquement les lignes contenant Erreur et affichez
également leur numéro de ligne.

6.Filtrez uniquement les lignes où le mot Erreur apparaît au début de la
ligne.

**<u>Corrections Exercices :</u>**

<u>Exercice 1 : Explorer un répertoire avec ls</u>

> **1.** **Affichez** **la** **liste** **des** **fichiers** **et**
> **dossiers** **dans** **votre** **répertoire** **personnel.**
>
> **Commande** : ls
>
> **Correction** : Afficher simplement les noms des fichiers et dossiers
> du répertoire courant.
>
> **2.** **Affichez** **la** **liste** **des** **fichiers** **avec**
> **leurs** **détails** **(permissions,** **taille,** **propriétaire,**
> **etc.).**
>
> **Commande** :ls -l
>
> **Correction** : Affiche des détails comme les permissions) : Affiche
> des détails comme les permissions ( drwxr-xr-x), le propriétaire, la
> taille et la date de modification.
>
> **3.** **Affichez** **uniquement** **les** **fichiers** **cachés.**
>
> **Commande** :ls -a
>
> **Correction** : Liste aussi les fichiers cachés (ceux qui commencent
> par . comme .bashrc).
>
> **4.** **Affichez** **les** **fichiers** **triés** **par** **taille.**
>
> **Commande** :ls -S
>
> **Correction** : Trier les fichiers du plus grand au plus petit.
>
> **5.** **Affichez** **la** **liste** **des** **fichiers** **avec**
> **leurs** **tailles** **au** **format** **lisible** **(K,** **M,**
> **G).**
>
> **Commande** : ls -lh
>
> **Correction** : Ajout d'une unité (K, M, G) pour rendre les tailles
> plus compréhensibles.

<u>Exercice 2 : Créer des fichiers et des dossiers avec mkdir et
touch</u>

> **1.** **Créez** **un** **répertoire** **nommé** **projet** **dans**
> **votre** **dossier** **personnel.**
>
> **Commande** : mkdir projet
>
> **2.** **Accédez** **à** **ce** **répertoire.**
>
> **Commande** : cd projet
>
> **3.** **Dans** **projet,** **crée** **trois** **sous-dossiers** **:**
> **docs,** **scripts,** **logs.**
>
> **Commande** : mkdir docs scripts logs
>
> **4.** **Dans** **le** **dossier** **docs,** **créez** **un**
> **fichier** **nommé** **README.txt.**
>
> **Commande** : touch docs/README.txt
>
> **5.** **Dans** **le** **dossier** **scripts,** **créez** **un**
> **fichier** **install.sh.**
>
> **Commande** : touch scripts/install.sh

<u>Exercice 3 : Créer un utilisateur et gérer ses droits</u>

> **1.** **Créez** **un** **nouvel** **utilisateur** **nommé**
> **devuser.**
>
> **Commande** :sudo adduser devuser
>
> **Correction** : Cette commande crée un utilisateur et demande un mot
> de passe.
>
> **2.** **Définissez** **un** **mot** **de** **passe** **pour**
> **devuser.**
>
> **Commande** : Lors de la création, le système demandera un mot de
> passe. (Sinon, utilisez : sudo passwd devuser)
>
> **3.** **Vérifiez** **que** **l'utilisateur** **a** **bien** **été**
> **créé.**
>
> **Commande** :cat /etc/passwd \| grep devuser
>
> **Correction** : Cette commande affiche l'entrée de l'utilisateur dans
> le fichier /etc/passwd.
>
> **4.** **Accordez-lui** **les** **droits** **de** **lecture** **et**
> **d'écriture** **sur** **le** **dossier** **projet.**
>
> **Commande** : sudo chown -R devuser : devuser ~/projet sudo chmod -R
> 755 ~/projet
>
> **Correction** :chownchangez le propriétaire du dossier et de son
> contenu. chmod755 donne les permissions ( rwxr-xr-x).

<u>Exercice 4 : Déplacer un fichier vers le dossier de l'utilisateur</u>

> **1.** **Déplacez** **le** **fichier** **install.shvers** **le**
> **dossier** **personnel** **de** **devuser.**
>
> **Commande** :sudo mv ~/projet/scripts/install.sh /home/devuser/
>
> **2.** **Vérifiez** **que** **le** **fichier** **a** **bien** **été**
> **déplacé.**
>
> **Commande** :ls -l /home/devuser/
>
> **Correction** : Cette commande affiche les fichiers présents dans le
> dossier de devuser.
>
> **3.** **Changez** **le** **propriétaire** **du** **fichier** **pour**
> **que** **devuseren** **ait** **le** **contrôle.**

**Commande** : sudo chown devuser:devuser /home/devuser/install.sh

<u>Exercice 5 : Rechercher du texte avec grep</u>

> **1.** **Créez** **un** **fichier** **logfile.txtet** **ajoutez-y**
> **du** **texte.**
>
> **Commande** : echo -e "Erreur : connexion échouée\nSuccès :
> utilisateur connecté\nErreur : accès refusé\nInfo : mise à jour
> effectuée" \> logfile.txt
>
> **2.** **Affichez** **toutes** **les** **lignes** **contenant** **le**
> **mot** **Erreur.**
>
> **Commande** :grep "Erreur" logfile.txt
>
> **3.** **Affichez** **toutes** **les** **lignes** **contenant**
> **Succès,** **en** **ignorant** **la** **casse.**
>
> **Commande** :grep -i "succès" logfile.txt
>
> **4.** **Comptez** **le** **nombre** **de** **lignes** **contenant**
> **Info.**
>
> **Commande** :grep -c "Info" logfile.txt
>
> **5.** **Affichez** **les** **lignes** **contenant** **Erreuravec**
> **leur** **numéro.**
>
> **Commande** :grep -n "Erreur" logfile.txt
>
> **6.** **Affichez** **uniquement** **les** **lignes** **où**
> **Erreurapparaissent** **au** **début.**
>
> **Commande** :grep "^Erreur" logfile.txt

<u>Exercice 6 : Explorer les pages du manuel avec man</u>

> **1.** **Affichez** **la** **documentation** **de** **la**
> **commande** **ls.**
>
> **Commande** : man ls
>
> **2.** **Trouvez** **l'option** **pour** **afficher** **les**
> **fichiers** **cachés** **avec** **ls.**
>
> **Réponse** : L'option -aest indiquée dans man ls.
>
> **3.** **Affichez** **la** **documentation** **de** **la**
> **commande** **mkdir.**
>
> **Commande** : man mkdir
>
> **4.** **Trouvez** **l'option** **pour** **créer** **un** **dossier**
> **avec** **ses** **sous-dossiers** **en** **une** **seule**
> **commande.**
>
> **Réponse** : L'option -pest indiquée dans man mkdir.
>
> **5.** **Affichez** **la** **documentation** **de** **grep.**
>
> **Commande** : man grep
>
> **6.** **Fermez** **man** **proprement** **sans** **CTRL+C.**
>
> **Commande** : Appuyez sur q.
>
> **7.** **Affichez** **uniquement** **les** **5** **premières**
> **lignes** **de** **la** **documentation** **de** **chmod.**
>
> **Commande** : man chmod \| head -n 5
>
> **8.** **Trouvez** **une** **alternative** **à** **man** **afficher**
> **la** **documentation** **d'une** **commande.**
>
> **Commande** : help cd (fonctionne avec les commandes intégrées au
> shell).
