# Projet_ TinyML 

## Projet 1 : Jalaleddine OUICH
En se basant sur les étapes du git suivant : https://github.com/walid213/tinyml-workshop

A l'aide de l'accelerometre, j'ai effectué des mouvements qui correspond aux signes yes/no.
Le mécanisme développé sera testé à l'aide de 3 questions qui seront posés à l'intermédiaire du port série.  

Vous trouverez dans Projet 1 :  
-le fichier "model.h" d'entrainement et les fichiers "yes.csv" et "no.csv"  
-le code source IMU_Classifier.ino utilisé pour le test et les questions.  

Résultat :  
  
![test.png](https://github.com/JalaleddineOUICH/Projet_IA/blob/main/Projet_1/test.png)  
  
  
## Projet 2 :  Jalaleddine OUICH | Elmehdi BAAZIZ
Le but c'est d'entrainer un modèle de reconnaissance des mots suivants : Résistance, Microncontrolleur, Bruit de fond.  
Déploiment du modèle sur une carte Arduino.  
Utilisez le mécanisme développé pour faire clignoter la led graduellement à chaque fois qu’on prononce un mot particulier.   
En suivant les étapes du [Tutorial](https://docs.edgeimpulse.com/docs/tutorials/responding-to-your-voice), on a opté à deux méthodes pour exécuter le programme :  
-Sur le terminal en uttilisant la commande *edge-impulse-run-impulse*  
-Sur l'IDE arduino.

## Projet Final : Skin Cancer Detection 

L'objectif de ce projet est de réaliser une classification d'images pour la détection du cancer de la peau en utilisant la carte Arduino Nano 33 Sense BLE et un module caméra.  
L'aspect le plus crucial du projet est la création de la base de données. Les images de cancer ont été obtenues sur le site [Kaggle] (https://www.kaggle.com/datasets/nodoubttome/skin-cancer9-classesisic), spécifiquement pour le cancer de la peau appelé "mélanome". La base de données contient deux classes étiquetées "safe_skin" et "cancer_skin".  

# Choix du modèle
