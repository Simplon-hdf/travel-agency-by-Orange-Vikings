# Dictionnaire de données

| Nom de classe | Nom court               | Nom complet                     | Type | Longueur | Commentaire    |
| ------------- | ------------------      | ------------------------------- | ---- | -------- | -------------- |
|**Client**     |cli_id                   |Numéro du client.                |AN    |76        |obligatoire     |
|               |cli_lastname             |Nom du client.                   |A     |6         |obligatoire     | 
|               |cli_firstname            |Prenom du client                 |A     |76        |obligatoire     |
|               |cli_birth                |Date d'anniversaire.             |Date  |          |obligatoire     |
|               |cli_gender               |Genre du client                  |A     |76        |obligatoire     |
|               |cli_mail                 |Mail du client                   |AN    |50        |obligatoire     |
|               |cli_phone                |Numéro telephone client          |N     |20        |oligatoire      |  
|**Booking**    |booking_id               |Numéro de la réservation         |AN    |76        |obligatoire     |
|               |booking_class            |Option de classe                 |A     |50        |obligatoire     |
|               |booking_date             |Date de réservation              |Date  |12        |obliagtoire     |
|**Passenger**  |pass_id                  |Numéro du passager               |AN    |76        |obligatoire     |   
|               |pass_lastname            |Nom du passager                  |A     |50        |obligatoire     |
|               |pass_firstname           |Prénom du passager               |A     |50        |obligatoire     |
|               |pass_email               |Email du passager                |AN    |50        |obligatoire     |
|               |pass_passport            |Passeport passager               |AN    |50        |facultatif      |
|               |pass_gender              |Genre de passager                |A     |50        |facultatif      |
|               |pass_phone               |Numéro de telephone du passager  |N     |50        |facultatif      |
|**Flight**     |flight_id                |Numéro du vol                    |AN    |50        |obligatoire     |
|               |flight_departuretime     |Heure de départ d'un vol         |N     |10        |obligatoire     |
|               |flight_arrivaltime       |Heure d'arrivée d'un vol         |N     |10        |obligatoire     |
|               |flight_placeOfDeparture  |Lieu de départ                   |A     |50        |obligatoire     |
|               |flight_arrivalLocation   |Lieu d'arriver                   |A     |50        |obligatoire     |
|**City**       |city_id                  |Numéro de la ville               |AN    |50        |obligatoire     |
|               |city_name                |Nom de la ville                  |A     |50        |obligatoire     |
|               |city_zipcode             |Code postale de la ville         |N     |10        |obligatoire     |
|**Country**    |Country_id               |Numéro du pays                   |AN    |50        |obligatoire     |
|               |country_name             |Nom du pays                      |A     |50        |obligatoire     |
|**Airport**    |airport_id               |Numéro de l'aéroport             |AN    |76        |obligatoire     |
|               |airport_name             |Nom de l'aéroport                |A     |50        |obligatoire     |
|               |airport_address          |Adresse de l'aéroport            |AN    |76        |obligatoire     |
|               |aiport_gate              |Numéro de la porte d'embarquement|N     |10        |obligatoire     |
|               |airport_terminal         |Numéro du terminal               |N     |10        |obligatoire     |
|**Airline**    |airline_id               |Numéro de la compagnie           |AN    |76        |obligatoire     |
|               |airline_name             |Nom de la compagnie              |A     |50        |obligatoire     |
|**Plane**      |plane_id                 |Numéro de l'avion                |N     |50        |obligatoire     |
|               |plane_model              |model de l'avion                 |AN    |50        |obligatoire     |
|               |plane_capacity           |Capacité de places dans l'avion  |N     |3         |obligatoire     |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |
|               |         |                |    |        | |







<!-- 
A/Alphabétique : composé uniquement de lettre a/A z/Z

N/Numérique : composé de nombre 

AN/AlphaNumérique : lettre et nombre 

Date : format "AAAA-MM-JJ"

Booléan : vrai ou faux  -->