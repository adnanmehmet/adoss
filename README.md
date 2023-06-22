# adoss
adoss
-- Veritabanı oluşturma
CREATE DATABASE mydatabase;

-- Kullanılacak veritabanını seçme
USE mydatabase;

-- Tablo oluşturma
CREATE TABLE customers (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    email VARCHAR(50)
);

-- Veri ekleme
INSERT INTO customers (id, name, email)
VALUES (1, 'John Doe', 'john@example.com'),
       (2, 'Jane Smith', 'jane@example.com'),
       (3, 'Mike Johnson', 'mike@example.com');

-- Veri sorgulama
SELECT * FROM customers;

-- Tablo güncelleme
UPDATE customers SET email = 'john.doe@example.com' WHERE id = 1;

-- Tablo silme
DROP TABLE customers;

-- Veritabanını silme
DROP DATABASE mydatabase;
