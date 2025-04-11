# Script SQL ⛁

## Table Client

```SQL
CREATE TABLE Customer(
   customer_id UUID PRIMARY KEY,
   customer_lastname VARCHAR(50) NOT NULL,
   customer_firstname VARCHAR(50) NOT NULL,
   customer_mail VARCHAR(64) NOT NULL UNIQUE,
   customer_birth DATE NOT NULL,
   customer_phone VARCHAR(10) NULL UNIQUE,
   customer_password VARCHAR(128) NOT NULL
);
```

## Table Passager

```SQL
CREATE TABLE Passenger(
   passenger_id UUID PRIMARY KEY,
   passenger_lastname VARCHAR(50) NOT NULL,
   passenger_firstname VARCHAR(50) NOT NULL,
   passenger_mail VARCHAR(64) UNIQUE NULL,
   passenger_passport VARCHAR(9) NOT NULL,
   passenger_gender CHECK(passenger_gender IN ('Male', 'Female', 'Other')) NULL,
   passenger_phone VARCHAR(10) NULL,
   passenger_type CHECK(passenger_type IN ('Adult', 'Kid', 'Baby')) NOT NULL
);
```

## Table Compagnie

```SQL
CREATE TABLE Airline(
   airline_id UUID PRIMARY KEY,
   airline_name VARCHAR(50) NOT NULL UNIQUE
);
```
