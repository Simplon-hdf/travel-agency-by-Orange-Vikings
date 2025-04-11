# Dictionnaire de données

| Nom de classe   | Nom court                    | Nom complet                      | Type | Longueur | Commentaire     |
| -------------   | -----------------------      | -------------------------------- | ---- | -------- | --------------- |
| **Customer**    | customer_id                  | Numéro du client                 | AN   | 36       | obligatoire     |
|                 | customer_lastname            | Nom du client                    | A    | 50       | obligatoire     |
|                 | customer_firstname           | Prénom du client                 | A    | 50       | obligatoire     |
|                 | customer_birth               | Date d'anniversaire              | Date | 12       | obligatoire     |
|                 | customer_password            | Mot de passe client              | A    | 128      | obligatoire     |
|                 | customer_mail                | Mail du client                   | AN   | 64       | obligatoire     |
|                 | customer_phone               | Numéro téléphone client          | N    | 15       | facultatif      |
| **Booking**     | booking_id                   | Numéro de la réservation         | AN   | 36       | obligatoire     |
|                 | booking_class                | Option de classe                 | A    | 10       | obligatoire     |
|                 | booking_date                 | Date de réservation              | Date | 12       | obligatoire     |
|                 | booking_seatnumber           | Place d'avion                    | AN   | 4        | obligatoire     |
| **Passenger**   | passenger_id                 | Numéro du passager               | AN   | 36       | obligatoire     |
|                 | passenger_lastname           | Nom du passager                  | A    | 50       | obligatoire     |
|                 | passenger_firstname          | Prénom du passager               | A    | 50       | obligatoire     |
|                 | passenger_email              | Email du passager                | AN   | 64       | facultatif      |
|                 | passenger_passport           | Passeport passager               | AN   | 9        | facultatif      |
|                 | passenger_gender             | Genre du passager                | A    | 1        | facultatif      |
|                 | passenger_phone              | Numéro de téléphone du passager  | N    | 15       | facultatif      |
| **Flight**      | flight_id                    | Numéro du vol                    | AN   | 36       | obligatoire     |
|                 | flight_departuretime         | Heure de départ d'un vol         | N    | 10       | obligatoire     |
|                 | flight_arrivaltime           | Heure d'arrivée d'un vol         | N    | 10       | obligatoire     |
| **City**        | city_id                      | Numéro de la ville               | AN   | 36       | obligatoire     |
|                 | city_name                    | Nom de la ville                  | A    | 50       | obligatoire     |
|                 | city_zipcode                 | Code postal de la ville          | N    | 10       | obligatoire     |
| **Country**     | country_id                   | Numéro du pays                   | AN   | 36       | obligatoire     |
|                 | country_name                 | Nom du pays                      | A    | 50       | obligatoire     |
| **Airport**     | airport_id                   | Numéro de l'aéroport             | AN   | 36       | obligatoire     |
|                 | airport_name                 | Nom de l'aéroport                | A    | 50       | obligatoire     |
|                 | airport_address              | Adresse de l'aéroport            | AN   | 250      | obligatoire     |
|                 | airport_gate                 | Numéro de la porte d'embarquement| AN   | 5        | obligatoire     |
|                 | airport_terminal             | Numéro du terminal               | AN   | 5        | obligatoire     |
| **Airline**     | airline_id                   | Numéro de la compagnie           | AN   | 36       | obligatoire     |
|                 | airline_name                 | Nom de la compagnie              | A    | 50       | obligatoire     |
| **Plane**       | plane_id                     | Numéro de l'avion                | N    | 36       | obligatoire     |
|                 | plane_model                  | Modèle de l'avion                | AN   | 50       | obligatoire     |
|                 | plane_capacity               | Capacité de places dans l'avion  | N    | 3        | obligatoire     |
