Question 1
1.Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.
The relationship between the "Product" and "Product_Category" entities is that of a one-to-many relationship. This means that each product belongs to one product category, but a product category can have multiple products associated with it. This relationship is established through the "category_id" foreign key in the "Product" table, which references the "id" primary key in the "Product_Category" table.

Question 2
2. How could you ensure that each product in the "Product" table has a valid category assigned to it?
To ensure that each product in the "Product" table has a valid category assigned to it, you can enforce referential integrity by setting up a foreign key constraint between the "category_id" column in the "Product" table and the "id" column in the "Product_Category" table. This constraint will ensure that every value in the "category_id" column of the "Product" table must exist in the "id" column of the "Product_Category" table, thereby guaranteeing that each product is associated with a valid category. Additionally, you can also include checks and validation logic in your application code to verify that a category is assigned to each product before it is inserted or updated in the database.

