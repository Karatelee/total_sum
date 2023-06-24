CREATE TABLE products(
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    price INT,
    quantity INT
);

INSERT INTO products(price,quantity) VALUES(10000, 2),
    (25000, 3),
    (30000, 2),
    (5000, 6),
    (20000, 2),
    (90000, 0),
    (10000, 1);
    (50001, 1),
    (30000, 10);
SELECT id, price * quantity AS total_sum
FROM products
ORDER BY  total_sum DESC
limit 3;
# total_sum
