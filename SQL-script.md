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
