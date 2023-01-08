# Projet_ TinyML

## Projet 1 :
En se basant sur les étapes du git suivant : https://github.com/walid213/tinyml-workshop

A l'aide de l'accelerometre, j'ai effectué des mouvements qui correspond aux signes yes/no.
Le mécanisme développé sera testé à l'aide de 3 questions qui seront posés à l'intermédiaire du port série.  

Vous trouverez dans Projet 1 :  
-le fichier "model.h" d'entrainement et les fichiers "yes.csv" et "no.csv"  
-le code source IMU_Classifier.ino utilisé pour le test et les questions.  

Résultat :  
  
![test.png](https://github.com/JalaleddineOUICH/Projet_IA/blob/main/Projet_1/test.png)  
  
  
## Projet 2 :  Jalaleddine OUICH | Elmehdi BAAZIZ
On dois entrainer un modèle de reconnaissance des mots suivants : Résistance, Microncontrolleur, Bruit de fond.  
Déploiment du modèle sur une carte Arduino.  
Utilisez le mécanisme développé pour faire clignoter la led graduellement à chaque fois qu’on prononce un mot particulier. 
Le projet est upload dans le github de mon camarade : https://github.com/midoyondaime/Projet_AI_Embaque/tree/main/Project_2  
On a opté à deux méthodesp pour exécuter le programme :  
-Sur le terminal en uttilisant la commande *edge-impulse-run-impulse*  
-Sur l'IDE arduino.
