# Rainforest Bazaar
![](https://paymentweek.com/wp-content/uploads/2018/04/02Z76nz2Q5j0d9QU4..png)

## SQL Database Design Exercise: Rainforest Bazaar

**Objective:** Practice the first 3 normalization rules and understand one-to-many and many-to-many relationships.

---

### Initial Data:

Let's start with a single, unnormalized `Orders` table:


| OrderID | CustomerName | CustomerEmail       | ProductID | ProductName       | Quantity | Price  | OrderDate  | ShippingAddress                  |
|---------|--------------|---------------------|-----------|-------------------|----------|--------|------------|----------------------------------|
| 1       | John Doe     | john.doe@gmail.com  | 101       | Wireless Mouse    | 2        | 25.00  | 2023-06-10 | 123 Street, City, Country, 12345 |
| 2       | John Doe     | john.doe@gmail.com  | 102       | Laptop Sleeve     | 1        | 15.00  | 2023-06-11 | 123 Street, City, Country, 12345 |
| 3       | Mary Johnson | mary.johnson@yahoo.com | 103   | Portable Charger  | 3        | 20.00  | 2023-06-11 | 456 Avenue, City, Country, 56789 |
| 4       | Jane Smith   | jane.smith@hotmail.com | 101     | Wireless Mouse    | 1        | 25.00  | 2023-06-12 | 789 Lane, City, Country, 91234   |
| 5       | Jane Smith   | jane.smith@hotmail.com | 104     | Bluetooth Speaker | 2        | 35.00  | 2023-06-12 | 789 Lane, City, Country, 91234   |
| 6       | James Brown  | james.brown@gmail.com  | 105     | USB-C Cable       | 5        | 10.00  | 2023-06-12 | 321 Road, City, Country, 87654   |
| 7       | James Brown  | james.brown@gmail.com  | 103     | Portable Charger  | 1        | 20.00  | 2023-06-12 | 321 Road, City, Country, 87654   |
| 8       | Mary Johnson | mary.johnson@yahoo.com | 102     | Laptop Sleeve     | 2        | 15.00  | 2023-06-13 | 456 Avenue, City, Country, 56789 |
| 9       | Mary Johnson | mary.johnson@yahoo.com | 106     | HDMI Cable        | 1        | 10.00  | 2023-06-13 | 456 Avenue, City, Country, 56789 |
| 10      | John Doe     | john.doe@gmail.com  | 104       | Bluetooth Speaker | 1        | 35.00  | 2023-06-14 | 123 Street, City, Country, 12345 |
---

## Tasks:

1. **First Normal Form (1NF):** Convert the `Orders` table into first normal form by eliminating duplicate columns and ensuring each column contains only atomic (indivisible) values.

2. **Second Normal Form (2NF):** Convert the 1NF tables into second normal form by ensuring that all non-key columns are fully dependent on the primary key.

3. **Third Normal Form (3NF):** Convert the 2NF tables into third normal form by ensuring that all columns are directly dependent on the primary key, and not on other columns.

4. **Relationships:** Define the one-to-many and many-to-many relationships between your tables. As a hint, consider the following:
    - One customer can place many orders.
    - One product can be included in many orders.
    - An order can include many products.

