# Projet-c
Description du Code : Gestionnaire de Réservations de Bus

Ce code C propose un système de gestion des réservations de bus, avec des fonctionnalités distinctes pour les administrateurs et les voyageurs. Le programme utilise des fichiers texte pour stocker les informations des voyageurs et les détails des réservations.

Structures de données :

Voyageur (struct voyageur) :

nom_v, prenom_v : Nom et prénom du voyageur.
id_v : Identifiant unique du voyageur.
N_tel : Numéro de téléphone du voyageur.
age : Âge du voyageur.
Bus (struct bus) :

id_bus : Identifiant unique du bus.
nb_places : Nombre de places dans le bus.
puissance : Puissance du moteur du bus.
suiv : Pointeur vers le bus suivant.
Réservation (struct reservation) :

v : Structure de type voyageur pour stocker les détails du voyageur.
b : Structure de type bus pour stocker les détails du bus.
depart, arrive : Villes de départ et d'arrivée de la réservation.
date : Date de la réservation.
N_res : Numéro de réservation unique.
prix : Coût de la réservation.
heur_depart, heur_arrive : Heures de départ et d'arrivée.
Fonctions Principales :

ajouter_bus : Ajoute un nouveau bus à la liste.

nbr_des_bus : Calcule le nombre de bus dans la liste.

supprimer_bus : Supprime un bus de la liste en fonction de son identifiant.

enregistrer_voyageur : Enregistre les détails d'un voyageur dans un fichier.

creer_compte : Crée un nouveau compte voyageur avec un identifiant unique.

lire_voyageur : Lit les détails d'un voyageur à partir du fichier.

modifier_compte : Modifie les détails d'un voyageur en fonction de l'identifiant et du champ spécifié.

afficherVoyageurs : Affiche la liste des voyageurs enregistrés.

reserver : Permet à un voyageur de faire une réservation.

modifier_reservation : Fonction à implémenter pour la modification des réservations.

afficher_detail_bus : Affiche les détails de tous les bus enregistrés.

Fonctionnalités de l'Application :

Mode Administrateur :

Ajouter un nouveau bus.
Supprimer un bus existant.
Afficher la liste des bus.
Afficher la liste des voyageurs.
Mode Voyageur :

Effectuer une réservation.
Modifier les détails du compte (nom, prénom, numéro de téléphone, âge).
Utilisation du Programme :

Le programme commence en demandant à l'utilisateur de choisir entre le mode administrateur, le mode voyageur, ou de quitter.
En mode administrateur, l'utilisateur peut effectuer différentes opérations sur les bus.
En mode voyageur, l'utilisateur peut effectuer des réservations et modifier son compte.
Les informations des voyageurs sont stockées dans le fichier "voyageurs.txt".
