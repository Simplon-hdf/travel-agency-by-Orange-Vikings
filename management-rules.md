# Règles de Gestion (Règles Métier) 📋✨

---

## 1. Vols ✈️

- **RG1** : Un vol appartient obligatoirement à une compagnie aérienne.
- **RG2** : Un vol possède un aéroport de départ et un aéroport d'arrivée.
- **RG3** : Un vol a une date et une heure de départ, ainsi qu'une date et une heure d'arrivée.
- **RG4** : Un vol peut être lié à plusieurs réservations.
- **RG5** : Un vol peut être modifié par sa compagnie.
- **RG6** : Un vol peut être annulé par sa compagnie.
- **RG7** : Un vol doit avoir un statut.
- **RG8** : Un vol doit avoir une durée de vol.
- **RG9** : Un vol doit avoir un numéro de vol.
- **RG10** : Un vol doit être lié à un avion.

---

## 2. Réservations 🎫

- **RG11** : Une réservation doit être effectuée par un client.
- **RG12** : Une réservation doit concerner un ou plusieurs vols.
- **RG13** : Une réservation est liée à un seul client.
- **RG14** : Une réservation possède un numéro de réservation.
- **RG15** : Une réservation peut être modifiée, confirmée ou annulée.
- **RG16** : Une réservation n'est confirmée qu'après validation du paiement.
- **RG17** : Une réservation contient un ou plusieurs passagers, chacun avec un numéro de siège attribué.
- **RG18** : Une réservation ne peut être créée que si le vol est encore ouvert à la réservation.
- **RG19** : Une réservation peut comporter une ou plusieurs escales.
- **RG20** : Une réservation doit avoir les informations du/des passager(s).
- **RG21** : Une réservation peut contenir plusieurs options de classes.
- **RG22** : Une réservation doit avoir un prix.
- **RG23** : Une réservation doit envoyer une notification de confirmation.
- **RG24** : Une réservation doit contenir un ou plusieurs billets de vol.

---

## 3. Passagers 👨‍👩‍👧‍👦

- **RG25** : Un passager doit avoir les informations suivantes :
  - Nom
  - Prénom
  - Date de naissance
  - Passeport (Optionnel)
  - Genre (Optionnel)
  - Numéro de téléphone (Optionnel)
- **RG26** : Un passager est lié à un vol et à un numéro de siège.
- **RG27** : Un passager est lié à une réservation et un billet.

---

## 4. Compagnies Aériennes 🏢

- **RG28** : Une compagnie aérienne peut :
  - Ajouter un vol
  - Modifier un vol
  - Annuler un vol
  - Ouvrir ou fermer un vol à la réservation
- **RG29** : Une compagnie aérienne doit avoir un ou plusieurs avions.
- **RG30** : Une compagnie aérienne doit avoir un nom.
- **RG31** : Une compagnie aérienne peut proposer des vols.

---

## 5. Aéroports ✈️

- **RG32** : Un aéroport doit avoir un nom.
- **RG33** : Un aéroport doit avoir une localisation (Pays, Ville, Adresse).
- **RG34** : Un aéroport peut desservir une ou plusieurs villes.
- **RG35** : Un aéroport peut être défini comme aéroport de départ, d'arrivée ou d'escale.
- **RG36** : Un aéroport doit avoir un statut (ouvert ou fermé).
- **RG37** : Un aéroport doit avoir une ou plusieurs portes d'embarquement.
- **RG38** : Un aéroport doit avoir une ou plusieurs pistes.
- **RG39** : Un aéroport doit avoir un code IATA.
- **RG40** : Un aéroport doit avoir un code OACI.

---

## 6. Client (achat) 💰

- **RG41** : Un client doit s'incrire en saisisant les information suivant :
  - Nom
  - Prénom
  - Genre
  - Date d'anniversaire
  - Numéro de téléphone
  - Email
  - Mot de passe
- **RG42** : Un client doit avoir un compte.
- **RG43** : Un client peut se connecter.
- **RG44** : Un client peut se déconnecter.
- **RG45** : Un client peut rechercher un vol.
- **RG46** : Un client peut filtrer les résultats de la recherche.
- **RG47** : Un client peut consulter les détails d'un vol.
- **RG48** : Un client peut consulter ses réservations (actuelles, passées).
- **RG49** : Un client peut modifier ses données personnelles dans son compte.
- **RG50** : Un client peut supprimer son compte.
- **RG51** : Un client peut ajouter ou retirer un ou plusieurs passagers d'une réservation.
- **RG52** : Un client doit réserver.
- **RG53** : Un client doit saisir les informations du passager lors d'une réservation.
- **RG54** : Un client peut annuler une réservation.
- **RG55** : Un client doit saisir les coordonnées suivantes au moment du paiement :
  - Date de naissance
  - Adresse de facturation
  - Numéro de téléphone
  - Coordonnées bancaires
- **RG56** : Un client peut être un passager.
- **RG57** : Un client doit être un membre.

---

## 7. Avion 🛩️

- **RG58** : Un avion doit avoir des sièges avec des numéros uniques.
- **RG59** : Un avion a une capacité maximale (nombre de sièges).
- **RG60** : Un avion doit appartenir à une compagnie aérienne.
- **RG61** : Un avion peut être affecté à un vol.
- **RG62** : Un avion doit avoir un modèle.
- **RG63** : Un avion doit avoir un statut (en vol, stationné, hors service).

---

## 8. Agence 🏬

- **RG64** : L'agence doit avoir un nom.
- **RG65** : L'agence doit avoir une/des adresse(s).
- **RG66** : L'agence a des horaires d'ouverture et de fermeture.
- **RG67** : L'agence peut être contactée.
- **RG68** : L'agence doit avoir une adresse mail et un numéro de téléphone.
- **RG69** : L'agence peut vendre des réservations de vols.
