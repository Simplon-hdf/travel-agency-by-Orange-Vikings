# Règles de Gestion (Règles Métier)

---

## 1. Visiteur (non inscrit)

- **RG1** : Un visiteur peut rechercher un vol.
- **RG2** : Un visiteur peut filtrer les résultats de la recherche.
- **RG3** : Un visiteur peut consulter les détails d’un vol.
- **RG4** : Un visiteur peut créer un compte.
- **RG5** : Un visiteur peut contacter l'agence.
- **RG6** : Un visiteur peut obtenir des informations sur l'agence.
- **RG7** : Un visiteur peut s'inscrire, les informations obligatoires à fournir sont :
  - Email
  - Mot de passe
  - Genre
  - Nom
  - Prénom

---

## 2. Vols

- **RG8** : Un vol appartient obligatoirement à une compagnie aérienne.
- **RG9** : Un vol possède un aéroport de départ et un aéroport d’arrivée.
- **RG10** : Un vol a une date et une heure de départ, ainsi qu’une date et une heure d’arrivée.
- **RG11** : Un vol peut être lié à plusieurs réservations.
- **RG12** : Un vol peut être modifié par sa compagnie.
- **RG13** : Un vol peut être annulé par sa compagnie.
- **RG14** : Un vol doit avoir un statut.
- **RG15** : Un vol doit avoir une durée de vol.
- **RG16** : Un vol doit avoir un numéro de vol.
- **RG17** : Un vol doit être lié à un avion.

---

## 3. Réservations

- **RG18** : Une réservation doit être effectuée par un client.
- **RG19** : Une réservation doit concerner un ou plusieurs vols.
- **RG20** : Une réservation est liée à un seul client.
- **RG21** : Une réservation possède un numéro de réservation.
- **RG22** : Une réservation peut être modifiée, confirmée ou annulée.
- **RG23** : Une réservation n’est confirmée qu’après validation du paiement.
- **RG24** : Une réservation contient un ou plusieurs passagers, chacun avec un numéro de siège attribué.
- **RG25** : Une réservation ne peut être créée que si le vol est encore ouvert à la réservation.
- **RG26** : Une réservation peut comporter une ou plusieurs escales.
- **RG27** : Une réservation doit avoir les informations du/des passager(s).
- **RG28** : Une réservation peut contenir plusieurs options de classes.
- **RG29** : Une réservation doit avoir un prix.
- **RG30** : Une réservation doit envoyer une notification de confirmation.
- **RG31** : Une réservation doit contenir un ou plusieurs billets de vol.

---

## 4. Passagers

- **RG32** : Un passager doit avoir les informations suivantes :
  - Nom
  - Prénom
  - Date de naissance
  - Passeport (Optionnel)
  - Genre (Optionnel)
  - Numéro de téléphone (Optionnel)
- **RG33** : Un passager est lié à un vol et à un numéro de siège.
- **RG34** : Un passager est lié à une réservation et un billet.

---

## 5. Compagnies Aériennes

- **RG35** : Une compagnie aérienne peut :
  - Ajouter un vol
  - Modifier un vol
  - Annuler un vol
  - Ouvrir ou fermer un vol à la réservation
- **RG36** : Une compagnie ne peut modifier ou annuler un vol.
- **RG37** : Une compagnie aérienne doit avoir un ou plusieurs avions.
- **RG38** : Une compagnie aérienne peut proposer des vols.
- **RG39** : Une compagnie aérienne doit avoir un nom.
- **RG40** : Une compagnie aérienne doit avoir un ou plusieurs avions.
- **RG41** : Une compagnie aérienne peut proposer des vols.

---

## 6. Aéroports

- **RG42** : Un aéroport doit avoir un nom.
- **RG43** : Un aéroport doit avoir une localisation (Pays, Ville, Adresse).
- **RG44** : Un aéroport peut desservir une ou plusieurs villes.
- **RG45** : Un aéroport peut être défini comme aéroport de départ, d’arrivée ou d’escale.
- **RG46** : Un aéroport doit avoir un statut (ouvert ou fermé).
- **RG47** : Un aéroport doit avoir un ou plusieurs ports d'embarquement.
- **RG48** : Un aéroport doit avoir une ou plusieurs pistes.
- **RG49** : Un aéroport doit avoir un IATA.
- **RG50** : Un aéroport doit avoir un OACI.

---

## 7. Membre (inscrit)

- **RG51** : Un membre doit avoir un compte.
- **RG52** : Un membre peut se connecter.
- **RG53** : Un membre peut se déconnecter.
- **RG54** : Un membre peut rechercher un vol.
- **RG55** : Un membre peut filtrer les résultats de la recherche.
- **RG56** : Un membre peut consulter les détails d’un vol.
- **RG57** : Un membre peut contacter l'agence.
- **RG58** : Un membre peut consulter ses réservations (actuelles, passées).
- **RG59** : Un membre peut modifier ses données personnelles dans son compte.
- **RG60** : Un membre peut supprimer son compte.
- **RG61** : Un membre peut être un client.

---

## 8. Client (achat)

- **RG62** : Un client peut ajouter ou retirer un ou plusieurs passagers à une réservation.
- **RG63** : Un client doit réserver.
- **RG64** : Un client doit saisir les informations du passager lors d'une réservation.
- **RG65** : Un client peut annuler une réservation.
- **RG66** : Un client doit avoir les coordonnées suivantes au moment du paiement :
  - Date de naissance
  - Adresse de facturation
  - Numéro de téléphone
  - Coordonnées bancaires
- **RG67** : Un client peut être un passager.
- **RG68** : Un client doit être un membre.

---

## 9. Avion

- **RG69** : Un avion doit avoir des sièges avec des numéros uniques.
- **RG70** : Un avion a une capacité maximale (nombre de sièges).
- **RG71** : Un avion doit appartenir à une compagnie aérienne.
- **RG72** : Un avion peut être affecté à un vol.
- **RG73** : Un avion doit avoir un modèle.
- **RG74** : Un avion doit avoir un statut (en vol, stationné, hors service).

---

## 10. Agence

- **RG75** : L'agence doit avoir un nom.
- **RG76** : L'agence doit avoir une/des adresse(s).
- **RG77** : L'agence a des horaires d'ouverture et de fermeture.
- **RG78** : L'agence peut être contactée.
- **RG79** : L'agence doit avoir une adresse mail et un numéro de téléphone.
- **RG80** : L'agence peut vendre des réservations de vols.
