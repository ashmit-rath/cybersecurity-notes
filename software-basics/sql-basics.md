# SQL Basics

SQL is used to interact with databases.

--------------------------------

## Select Data

SELECT * FROM users;

Get specific column
SELECT username FROM users;

--------------------------------

## Where Condition

SELECT * FROM users WHERE id=1;

SELECT * FROM users WHERE username='admin';

--------------------------------

## Insert Data

INSERT INTO users (username,password)
VALUES ('ash','1234');

--------------------------------

## Update Data

UPDATE users
SET password='newpass'
WHERE username='ash';

--------------------------------

## Delete Data

DELETE FROM users
WHERE username='ash';

--------------------------------

## Login Example

SELECT * FROM users
WHERE username='admin'
AND password='1234';

--------------------------------

## SQL Injection Example

' OR 1=1 --

Example:

SELECT * FROM users
WHERE username='' OR 1=1 --

This bypasses login
