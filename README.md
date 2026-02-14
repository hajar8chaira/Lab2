# LAB 2 : Rooting Android

# Step 1 : Rooter l'AVD :
1. Demarrer le serveur ADB avec privilege root et remonter en mode lecture et ecriture.

<p align="center"> <img src="images/im1.png" width="700"> </p>

2. Verification:
<p align="center"> <img src="images/im2.png" width="700"> </p>
<p align="center"> <img src="images/im4.png" width="500"> </p>

3. Journalisation:
<p align="center"> <img src="images/im5.png" width="700"> </p>
<p align="center"> <img src="images/im6.png" width="700"> </p>

# Step 2 : Fiche périmètre:

Application + version : DIVA (Damn Insecure and Vulnerable App) 
<p align="center"> <img src="images/im7.png" width="700"> </p>
– version installée sur l’AVD 
<p align="center"> <img src="images/im11.png" width="800"> </p>

Support : Émulateur Android - AVD Pixel_6 

Objectif : Comprendre le rooting et analyser ses impacts sur la sécurité de l’application

Données utilisées : Données fictives / environnement de test uniquement

Réseau : Réseau de test isolé (aucune interaction avec un environnement réel)

# Step 3: Démarrer un AVD propre:

<p align="center"> <img src="images/im7.1.png" width="500"> </p>
<p align="center"> <img src="images/im7.2.png" width="400"> </p>

# Step 4:  Installer et lancer l'app de test:
<p align="center"> <img src="images/im8.png" width="700"> </p>
<p align="center"> <img src="images/im9.png" width="700"> </p>
<p align="center"> <img src="images/im10.png" width="400"> </p>

# Step 5: Définir 3 scénarios simples:
##DIVA – Scénarios de test (ADB)
1. Scénario 1 — Ouvrir l’application Diva (Écran d’accueil)
##Objectif: Lancer DIVA et afficher l’écran principal.

-Revenir au Home Android:
<p align="center"> <img src="images/s1.png" width="700"> </p>

-Lancer l’application 
<p align="center"> <img src="images/s6-2.png" width="700"> </p>

-L’écran principal de DIVA s’affiche avec la liste des modules.
<p align="center"> <img src="images/s7-2.png" width="300"> </p>

2. Scénario 2 — Rechercher un item 
##Objectif : ouvrir la recherche et taper un texte toujours identique.
<p align="center"> <img src="images/s9.png" width="500"> </p>
<p align="center"> <img src="images/s10.png" width="500"> </p>
-Ouvrir la recherche:
<p align="center"> <img src="images/s11.png" width="500"> </p>

-Taper le texte exact:
<p align="center"> <img src="images/s12.png" width="300"> </p>

-Valider (Entrée):
<p align="center"> <img src="images/s13.png" width="500"> </p>
<p align="center"> <img src="images/s14.png" width="300"> </p>

3. Scénario 3 — Ouvrir une fiche détail et revenir:

##Objectif:Accéder à un LAPPLICATION  ET CHOISIR UN ITEM  puis revenir en arrière.

-Pour cliquer sur un item detail de lapplication :
<p align="center"> <img src="images/s16.png" width="300"> </p>

-Revenir en arriere:
<p align="center"> <img src="images/s17.png" width="300"> </p>

-L’écran détail s’affiche et Le bouton "Back" ramène à la liste principale


# Step 6:  Lire Android Security:

La sécurité Android repose sur plusieurs couches de protection.
Chaque application fonctionne dans une sandbox, ce qui signifie qu’elle est isolée des autres (comme une salle de classe fermée).
Le modèle de permissions contrôle l’accès aux ressources sensibles (caméra, stockage, micro), comme demander l’autorisation au professeur avant d’utiliser du matériel.
Le système garantit aussi l’intégrité globale, empêchant les modifications non autorisées du système.
Le rooting peut contourner ces protections en donnant un accès privilégié au système.
Comprendre ces couches aide à analyser les risques liés à la sécurité Android.
