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

## Table pays

```SQL
CREATE TABLE Country(
   country_id UUID PRIMARY KEY,
   country_name VARCHAR(50) NOT NULL UNIQUE
);
```

## Table Réservation

```SQL
CREATE TABLE Booking(
   booking_id UUID PRIMARY KEY,
   booking_class VARCHAR(10) CHECK(booking_class IN ('Economy','Business', 'First')) NOT NULL,
   booking_date TIMESTAMP NOT NULL,
   booking_seatnumber VARCHAR(4) NOT NULL UNIQUE,
   passenger_id UUID NOT NULL UNIQUE,
   customer_id UUID NOT NULL UNIQUE,
   FOREIGN KEY (passenger_id) REFERENCES Passenger(passenger_id),
   FOREIGN KEY (customer_id) REFERENCES Customer(customer_id)
);
```

## Table Avion

```SQL
CREATE TABLE Plane(
   plane_id UUID PRIMARY KEY,
   plane_capacity INT NOT NULL,
   plane_model VARCHAR(50) NOT NULL,
   airline_id UUID NOT NULL,
   FOREIGN KEY (airline_id) REFERENCES Airline(airline_id)

);
```

## Table Ville

```SQL
CREATE TABLE City(
   city_id UUID PRIMARY KEY,
   city_name VARCHAR(50) NOT NULL,
   city_zipcode VARCHAR(10) NOT NULL UNIQUE,
   country_id UUID NOT NULL,
   FOREIGN KEY (country_id) REFERENCES Country(country_id)
);
```

## Table Aéroport

```SQL
CREATE TABLE Airport(
   airport_id UUID PRIMARY KEY,
   airport_name VARCHAR(80) NOT NULL,
   airport_address VARCHAR(250) NOT NULL UNIQUE,
   airport_gate VARCHAR(5) NOT NULL,
   airport_terminal VARCHAR(5) NOT NULL,
   city_id UUID NOT NULL,
   FOREIGN KEY (city_id) REFERENCES City(city_id)
);
```

## Table Vol

```SQL
CREATE TABLE Flight(
   flight_id UUID PRIMARY KEY,
   flight_departuretime TIMESTAMPTZ NOT NULL,
   flight_arrivaltime TIMESTAMPTZ NOT NULL,
   arrival_airport_id UUID NOT NULL,
   plane_id UUID NOT NULL,
   FOREIGN KEY (departure_airport_id) REFERENCES Airport(airport_id),
   FOREIGN KEY (arrival_airport_id) REFERENCES Airport(airport_id),
   FOREIGN KEY (plane_id) REFERENCES Plane(plane_id)
);
```

## Table historique des réservations et vols

```SQL
CREATE TABLE Logs(
   flight_id UUID NOT NULL,
   booking_id UUID NOT NULL,
   PRIMARY KEY (flight_id, booking_id),
   FOREIGN KEY (flight_id) REFERENCES Flight(flight_id),
   FOREIGN KEY (booking_id) REFERENCES Booking(booking_id)
);
```
