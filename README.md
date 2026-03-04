# 🧸 PlushieShop

PlushieShop is a web application developed with Java, Spring Boot, and MySQL. It simulates a virtual store specializing in plush toys across multiple categories, integrating authentication, product management, shopping cart functionality, and user interaction features. The system was designed following course requirements and best practices in web development.

## ✨ Features

- 🔐 User Management
    - 📝 User registration system.
    - 🔑 Secure login authentication.
    - 🔒 Secure storage of sensitive data in the database.
    - 👤 Account-based access to the shopping cart.
- 🛍️ Product Browsing & Navigation
    - 📦 View full list of available products.
    - 🧸 Browse 4 main product categories.
    - 📂 Navigate through subcategories.
    - 🔎 Search products quickly using the search bar.
    - ❤️ Like/favorite products.
    - 🔁 Receive suggestions of similar products based on purchases.
    - 🌟 “Recommended” section with carousel of best-selling products.
    Each product includes:
        - 🖼️ Image
        - 🏷️ Name
        - 📏 Size
        - 🗂️ Category
        - 💲 Price
        - ❤️ Add-to-cart button (turns red when selected)
- 🛒 Shopping Cart & Payment
    - 🛍️ Add products to shopping cart.
    - 🗑️ Remove products from cart.
    - 💵 Automatic subtotal and total calculation.
    - 💳 Payment via credit or debit card.
    - ✅ Purchase confirmation message after successful transaction.
- 💬 Reviews & Communication
    - 📝 Users can leave reviews and comments.
    - 🤝 Contact seller or store representative for:
        - Questions
        - Complaints
        - General support

## 🖥️ Technologies Used

- 🎨 **Frontend:** CSS, HTML, Javascript  
- ☕ **Backend:** Java  
- 🚀 **Framework:** Spring Boot  
- 🌿 **Template Engine:** Thymeleaf  
- 🗄️ **Database:** MySQL  
- 🌐 **Server:** Apache  
- 🌱 **Version Control:** Git

## ⚙️ Installation

### 📋 Prerequisites

- 💻 [Apache NetBeans](https://netbeans.apache.org/front/main/index.html) (Recommended: Apache NetBeans 28)
- 🧰 [MySQL Workbench](https://www.mysql.com/products/workbench/)
- 🚀 [Spring Boot](https://spring.io/projects/spring-boot)

### 🔧 Configuration

1. 📥 Clone the repository:

   ```bash
   git clone https://github.com/Crisrod0912/PlushieShop_V1.git
   ```

2. 📂 Open the project folder in Apache Netbeans:

3. 🗄️ Import and execute the database dump:

   Import the `PlushieShop.sql` file into MySQL. After importing it, execute the script in your database.

4. 🔐 Configure database permissions:

   After importing the database, create a user and grant them the necessary permissions by running the following commands in the MySQL console:

   ```sql
   CREATE USER 'grupo5'@'%' IDENTIFIED BY 'clave_bd';
   
   GRANT ALL PRIVILEGES ON plushieShop.* to 'grupo5'@'%';
   
   FLUSH PRIVILEGES;
   ```

   Replace `'clave_bd'` with a more secure password if desired.

5. ⚙️ Update `application.properties`:

   Update the `src/main/resources/application.properties` file with your database configuration details:

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/plushieshop?useTimezone=true&serverTimezone=UTC
   spring.datasource.username=grupo5
   spring.datasource.password=clave_bd
   ```

6. ▶️ Run the project:

   - Click on "Run Project".

7. 🌐 Access the application in your web browser at `http://localhost:80`.

> [!NOTE]
> **Project Owner / Developer** 👨🏻‍💻  
>- Cristopher Rodríguez Fernández 
***
