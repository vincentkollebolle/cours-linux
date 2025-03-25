# TP Power Rangers – Paul Mysliwiec-Vilfeu

Tu es le gestionnaire des Power Rangers, je vais t’expliquer ce que tu dois faire. Si tu as du mal avec des commandes tu trouveras des informations supplémentaires avec man [commande].
1 – Pour commencer, vérifie où tu te trouves.
2 – Si tu n’y es pas déjà, va dans ton dossier personnel en une seule commande.
3 – Crée un dossier « equipe » pour les Power Rangers et vérifie qu’il a bien été créé.
4 – On va devoir recenser tous les Power Rangers. Va dans le dossier et crée un fichier rangerjaune.txt  .
5 – Modifie le fichier pour écrire « Je suis le power rangers jaune ». Tu peux y ajouter d’autres informations si tu veux, c’est sa carte d’identité dans le système.
6 – Rajoute les autres Power Rangers : rangerbleu / rangerrouge / rangerrose / rangernoir.
7 – Affiche le contenu de deux Power Rangers, ou plus, avec une seule commande.
8 – Lorsqu’ils sont en mission tu vas devoir les classer pour savoir s’ils sont à la base ou en mission. Crée un dossier mission et un dossier base.
9 – Les Power Rangers bleu, rose et rouge sont en mission et les Power Rangers noir et jaune sont à la base. Déplace-les à leur poste respectif, mission ou base.
10 – Pour s’assurer que le contenu est le bon, cherche le mot « rouge » dans le rangerrouge.txt
11 – Malheureusement, le ranger bleu a succombé à ses blessures. Supprime-le de l’équipe.
12 – Fais un rapport de 20 lignes pour comprendre comment le ranger bleu est mort. (Numérote juste les lignes de 1 à 20). Affiche les 10 premières lignes du rapport puis de même pour les 10 dernières.# TP Power Rangers – Paul Mysliwiec-Vilfeu


1 – Pour commencer, vérifie où tu te trouves. 
`pwd`
2 – Si tu n’y es pas déjà, va dans ton dossier personnel en une seule commande. 
`cd ~`
3 – Crée un dossier « equipe » pour les Power Rangers et vérifie qu’il a bien été créé.
`mkdir equipe puis ls`
4 – On va devoir recenser tous les Power Rangers. Va dans le dossier et crée un fichier rangerjaune.txt  . 
`cd equipe puis touch rangerjaune.txt`
5 – Modifie le fichier pour écrire « Je suis le power rangers jaune ». Tu peux y ajouter d’autres informations si tu veux, c’est sa carte d’identité dans le système.
`vim rangerjaune.txt puis pour quitter et enregistrer echap et :wq `
6 – Rajoute les autres Power Rangers : rangerbleu / rangerrouge / rangerrose / rangernoir.
`touch rangerxxx.txt`
7 – Affiche le contenu de deux Power Rangers, ou plus, avec une seule commande.
`cat ranger1.txt | cat ranger2.txt`
8 – Lorsqu’ils sont en mission tu vas devoir les classer pour savoir s’ils sont à la base ou en mission. Crée un dossier mission et un dossier base.
`mkdir mission et mkdir base`
9 – Les Power Rangers bleu, rose et rouge sont en mission et les Power Rangers noir et jaune sont à la base. Déplace-les à leur poste respectif, mission ou base.
`mv rangerxxx.txt [destination]`
10 – Pour s’assurer que le contenu est le bon, cherche le mot « rouge » dans le rangerrouge.txt
`grep « rouge » rangerrouge.txt  `
11 – Malheureusement, le ranger bleu a succombé à ses blessures. Supprime-le de l’équipe.
`rm rangerbleu.txt`
12 – Fais un rapport de 20 lignes pour comprendre comment le ranger bleu est mort. (Numérote juste les lignes de 1 à 20). Affiche les 10 premières lignes du rapport puis de même pour les 10 dernières.
`head [fichier] et tail [fichier]`
