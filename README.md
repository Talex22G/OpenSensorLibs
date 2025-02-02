# OpenSensorLibs

------------------------------------------------------------

Structure du dépôt
-

Chaque capteur ou actionneur doit être documenté et organisé dans un dossier spécifique portant son nom. La structure de chaque dossier doit être la suivante :

-📂 Nom_du_Capteur/

 ├── src/
 
 │   ├── capteur.c       # Fichier source contenant l'implémentation du capteur
 
 │   ├── capteur.h       # Fichier d'en-tête avec les déclarations des fonctions
 
 │   └── example.c       # Exemple de programme utilisant le capteur
 
 ├── README.md           # Documentation détaillant le fonctionnement et l'utilisation
 
------------------------------------------------------------

README.md
-

 Chaque dossier de capteur doit contenir un fichier README.md expliquant :

  -Description du capteur/actionneur : Informations générales sur son rôle et ses caractéristiques.

  -Dépendances : Bibliothèques nécessaires, protocoles utilisés (I2C, SPI, UART, etc.).

  -Son adresse si I2C.
  
------------------------------------------------------------

Normes de codage
-

Toutes les fonctions implémentées doivent inclure une en-tête de documentation expliquant leur rôle et leur utilisation. 

Exemple :

```c
/**
 * @brief Lit la température du capteur TMP36.
 * @return La température en degrés Celsius.
 */
float lire_temperature();
