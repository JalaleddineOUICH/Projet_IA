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
L'aspect le plus crucial du projet est la création de la base de données. Les images de cancer ont été obtenues sur le site [Kaggle](https://www.kaggle.com/datasets/nodoubttome/skin-cancer9-classesisic), spécifiquement pour le cancer de la peau appelé "mélanome". La base de données contient deux classes étiquetées "safe_skin" et "cancer_skin".  

### 1. Choix du modèle
Le choix d'un modèle est crucial pour ce projet. Nous devons garder à l'esprit la quantité de RAM qui est accessible avec l'Arduino Nano ble 33. Nous choisirons la famille de modèles MobileNet.  
![Image1.PNG](https://github.com/JalaleddineOUICH/Projet_IA/blob/main/Images/Image1.PNG) 
### 2. Entraînement 
Nous allons entraîner le modèle avec 2 méthodes différentes :  
#### 2.1. Edge Impulse  
#### L'acquisition de données :  
![Image2.PNG](https://github.com/JalaleddineOUICH/Projet_IA/blob/main/Images/Image2.PNG)  
#### Impulse :
![Image3.PNG](https://github.com/JalaleddineOUICH/Projet_IA/blob/main/Images/Image3.PNG)  
#### Test et déploiement du modèle :
Nous avons réussi à avoir un modèle relativement solide :  
![Image4.PNG](https://github.com/JalaleddineOUICH/Projet_IA/blob/main/Images/Image4.PNG) 
#### 2.2. Google Colab
En suivant les étapes de ce [Tutorial](https://gist.github.com/gheesung/eb0076e040ba53d5be2ad2db1c70cf82) sur google colab, nous obtenons les fichiers suivants après l'entraînement : 
![Image5.PNG](https://github.com/JalaleddineOUICH/Projet_IA/blob/main/Images/Image5.PNG) 
Nous avons modifié model_settings.cpp en changeant kNumChannels à 3 (pour rouge, vert et bleu) et kCategoryCount à 2 dans model_settings.h car nous avons 2 classes.

### Résultat
![Image6.jpg](https://github.com/JalaleddineOUICH/Projet_IA/blob/main/Images/Image6.jpg) 


