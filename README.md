# for database creation 

CREATE DATABASE your_db;
USE your_db;

CREATE TABLE users(
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    password VARCHAR(100) NOT NULL
);

SELECT * FROM users;

ALTER TABLE users ADD COLUMN role VARCHAR(10) NOT NULL DEFAULT 'user';

-----------------------------------

#installer:

pip install flask flask-mysqldb

-----------------------------------

#run this code

python app.py