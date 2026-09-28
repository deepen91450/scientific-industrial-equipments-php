<div align="center">

<!-- 🖼️ PLACEHOLDER: replace with your logo or banner, e.g. ./docs/banner.png -->
<!-- <img src="docs/banner.png" alt="Scientific & Industrial Equipments banner" width="720"> -->

# Scientific & Industrial Equipments

**A full-featured e-commerce web application for buying scientific and industrial equipment online, with a complete admin panel for managing products, users, and orders.**

![PHP](https://img.shields.io/badge/PHP-7-777BB4?logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-UI-7952B3?logo=bootstrap&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-CSS3-E34F26?logo=html5&logoColor=white)
<!-- Replace OWNER/REPO below with your GitHub path, then uncomment -->
<!-- ![License](https://img.shields.io/github/license/OWNER/scientific-industrial-equipments-php) -->
<!-- ![Last commit](https://img.shields.io/github/last-commit/OWNER/scientific-industrial-equipments-php) -->
<!-- ![Stars](https://img.shields.io/github/stars/OWNER/scientific-industrial-equipments-php?style=social) -->

</div>

---

## Table of Contents

- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Screenshots](#screenshots)
- [Getting Started](#getting-started)
- [System Design](#system-design)
- [Database Schema](#database-schema)
- [Project Structure](#project-structure)
- [Feasibility Study](#feasibility-study)
- [Project Timeline](#project-timeline)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)
- [References](#references)

---

## About

Buying equipment in person means visiting shop after shop, hunting for stock, and guessing at fair prices. **Scientific & Industrial Equipments** moves that process online.

Customers browse products, add them to a cart, and check out. Admins manage the catalog, users, and order fulfillment from a dedicated panel.

### Problems with the current system

- **Manual searching:** Customers must visit shops in person to find products.
- **Stock gaps:** Items are often unavailable, which forces a search at other shops.
- **Price opacity:** New customers do not know an item's real price and may overpay.

### How this project helps

- **Faster buying:** Browse many items at once and spend less time shopping.
- **Always open:** Order products at any time, from anywhere.
- **No reach limits:** A seller is no longer limited to the buyers near a physical store.
- **Flexible payment:** Pay by UPI, cash on delivery, or card on delivery.
- **Easy returns:** Return a product you do not like.

---

## Features

### User roles

| Role | Capabilities |
| --- | --- |
| **Visitor** | Browse and view available products. |
| **User** | Register, log in, view products, and purchase them. |
| **Admin** | Everything a user can do, plus add, edit, and remove products, and ship orders. |

### Highlights

- **Product browsing:** Browse the catalog and search for products.
- **Shopping cart:** Collect items in a cart and convert them into an order.
- **Checkout:** Provide a billing address and payment information to place an order.
- **Order notifications:** Customers receive a notification as soon as an order is placed.
- **Multiple payment modes:** UPI, cash on delivery, and card on delivery.
- **Product returns:** Users can return products they dislike.
- **Catalog management:** Admins add, edit, activate, deactivate, and delete products and categories.
- **User management:** Admins view and delete registered users.
- **Order management:** Admins review orders and ship them, with a confirmation mail sent to the customer.
- **Simple interface:** No special training is needed to use the system.

---

## Tech Stack

| Layer | Technology |
| --- | --- |
| **Backend** | PHP 7 |
| **Database** | MySQL |
| **Frontend** | HTML, CSS, Bootstrap |
| **Server** | Apache HTTP Server (via XAMPP) |
| **Editor** | Visual Studio Code (PHP IntelliSense) |
| **Browser** | Google Chrome |

---

## Screenshots

### Storefront

<table>
  <tr>
    <td align="center"><b>Homepage</b><br><img src="https://github.com/user-attachments/assets/ee68bf39-ff80-42e7-a438-9b043b864f2d" alt="Homepage" width="420"></td>
    <td align="center"><b>Product</b><br><img src="https://github.com/user-attachments/assets/3d28a28b-8e0e-4dd0-ac8f-905b3544c5a9" alt="Product page" width="420"></td>
  </tr>
  <tr>
    <td align="center"><b>Login</b><br><img src="https://github.com/user-attachments/assets/8bb8e102-ed4b-4473-a105-8c04b030bed5" alt="Login page" width="420"></td>
    <td align="center"><b>Register</b><br><img src="https://github.com/user-attachments/assets/0dd95755-6a23-4078-b5ab-fd6fcdc209d4" alt="Register page" width="420"></td>
  </tr>
  <tr>
    <td align="center"><b>Cart</b><br><img src="https://github.com/user-attachments/assets/bd35d8e3-6202-4112-a4b1-ebb752ebb442" alt="Shopping cart" width="420"></td>
    <td align="center"><b>Checkout</b><br><img src="https://github.com/user-attachments/assets/e84014ee-a851-4011-8ca6-03af56c89180" alt="Checkout page" width="420"></td>
  </tr>
</table>

### Admin panel

<table>
  <tr>
    <td align="center"><b>Admin Login</b><br><img src="https://github.com/user-attachments/assets/307afdfc-c180-4f62-aa35-e319507fbe36" alt="Admin login" width="420"></td>
    <td align="center"><b>Dashboard</b><br><img src="https://github.com/user-attachments/assets/5114fd60-2bb2-4a55-ae96-19cddabe77eb" alt="Admin dashboard" width="420"></td>
  </tr>
  <tr>
    <td align="center"><b>New Category</b><br><img src="https://github.com/user-attachments/assets/3f97dbd0-1a97-48dc-8220-511307095277" alt="New category" width="420"></td>
    <td align="center"><b>Products</b><br><img src="https://github.com/user-attachments/assets/a796622b-2766-44e8-a03f-00204bd69a36" alt="Products list" width="420"></td>
  </tr>
  <tr>
    <td align="center"><b>Add Product</b><br><img src="https://github.com/user-attachments/assets/8b255be5-41b8-421a-a96c-90c808bcb172" alt="Add product" width="420"></td>
    <td align="center"><b>Edit / Update Product</b><br><img src="https://github.com/user-attachments/assets/acc550cc-1c7f-4c87-86ae-8fc521d36d65" alt="Edit product" width="420"></td>
  </tr>
  <tr>
    <td align="center" colspan="2"><b>User Manager</b><br><img src="https://github.com/user-attachments/assets/f979f079-f316-4940-a286-857f1526d4fa" alt="User manager" width="420"></td>
  </tr>
</table>

---

## Getting Started

Follow these steps to run the project on your local machine.

### Prerequisites

| Requirement | Notes |
| --- | --- |
| **XAMPP** | Provides Apache, MySQL, and PHP. |
| **PHP 7** | Bundled with XAMPP. |
| **Google Chrome** | Or any modern browser. |
| **Visual Studio Code** | Optional. Use it with the PHP IntelliSense extension. |

**Recommended hardware:** Intel Core i3 @ 2 GHz, 4 GB RAM, 1 TB hard disk.

### Installation

**1. Clone the repository into your XAMPP web root**

The default configuration expects the project at `htdocs/php/ecom`.

```bash
cd C:/xampp/htdocs
mkdir php && cd php
git clone https://github.com/OWNER/scientific-industrial-equipments-php.git ecom
```

> Replace `OWNER` with the repository owner's GitHub username.

**2. Start the servers**

Open the XAMPP Control Panel and start **Apache** and **MySQL**.

**3. Create the database**

Create a MySQL database named `ecom` (for example, through phpMyAdmin at `http://localhost/phpmyadmin`). Then import the project's SQL file.

<!-- 📌 PLACEHOLDER: add the path of your SQL dump here, e.g. database/ecom.sql -->

The [database schema](#database-schema) below lists the tables the application expects.

**4. Check the connection settings**

The application connects using the values in `connection.inc.php`. Update them if your setup differs.

```php
$con = mysqli_connect("localhost", "root", "", "ecom");
define('SERVER_PATH', $_SERVER['DOCUMENT_ROOT'] . '/php/ecom/');
define('SITE_PATH', 'http://127.0.0.1/php/ecom/');
```

### Usage

1. Open **http://127.0.0.1/php/ecom/** in your browser to reach the storefront.
2. Register a user account, then browse products, add items to the cart, and check out.
3. Open the admin panel's `login.php` page and sign in with an admin account.
4. From the admin panel, manage **categories**, **products**, **users**, and **orders**.

---

## System Design

Click a diagram to expand it.

<details>
<summary><b>Event Table</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/2f248944-1569-4fb1-aa87-dd09bcf25be6" alt="Event table" width="800">
</details>

<details>
<summary><b>Entity Relationship (ER) Diagram</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/8d5bd54a-adb1-4e91-91ab-6ba515de3712" alt="ER diagram" width="800">
</details>

<details>
<summary><b>Class Diagram</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/b732f45b-edcc-45e5-9a89-2159e1d2105b" alt="Class diagram" width="800">
</details>

<details>
<summary><b>Activity Diagram</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/e464bd75-a046-447f-ac00-fffacfc17022" alt="Activity diagram" width="800">
</details>

<details>
<summary><b>Use Case Diagrams</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/08bdfa54-3bd2-44b8-8f51-2866f45b4e29" alt="Use case diagram 1" width="800">
<br><br>
<img src="https://github.com/user-attachments/assets/ff63c492-956f-4ccb-8157-16953634656d" alt="Use case diagram 2" width="800">
</details>

<details>
<summary><b>Sequence Diagrams (User and Admin)</b></summary>
<br>
<b>User</b><br>
<img src="https://github.com/user-attachments/assets/a9078d59-c8ea-4a30-9b63-991659fa8688" alt="User sequence diagram" width="800">
<br><br>
<b>Admin</b><br>
<img src="https://github.com/user-attachments/assets/73b01572-b6ab-4c3d-80c4-35aef6f1175f" alt="Admin sequence diagram" width="800">
</details>

<details>
<summary><b>Component Diagram</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/dce418e6-d9af-43e0-b841-c3599d0228a0" alt="Component diagram" width="800">
</details>

<details>
<summary><b>Deployment Diagram</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/b7249e74-e33b-464a-9094-d98ff0606b62" alt="Deployment diagram" width="800">
</details>

---

## Database Schema

<details>
<summary><b>Admin</b></summary>

| Field | Type | Size | Constraint |
| --- | --- | --- | --- |
| `id` | int | 11 | Primary key |
| `username` | varchar | 255 | Not null |
| `password` | varchar | 255 | Not null |
</details>

<details>
<summary><b>Users</b></summary>

| Field | Type | Size | Constraint |
| --- | --- | --- | --- |
| `id` | int | 11 | Primary key |
| `name` | varchar | 255 | Not null |
| `password` | varchar | 255 | Not null |
| `email` | varchar | 255 | Not null |
| `mobile` | int | 15 | Not null |
| `added_on` | datetime | - | Not null |
</details>

<details>
<summary><b>Categories</b></summary>

| Field | Type | Size | Constraint |
| --- | --- | --- | --- |
| `Category_id` | int | 11 | Primary key |
| `categories` | varchar | 255 | Not null |
| `status` | tinyint | 4 | Not null |
</details>

<details>
<summary><b>Product</b></summary>

| Field | Type | Size | Constraint |
| --- | --- | --- | --- |
| `Product_id` | int | 11 | Primary key |
| `Categories_id` | int | 11 | Foreign key |
| `name` | varchar | 255 | Not null |
| `mrp` | float | 255 | Not null |
| `price` | float | 255 | Not null |
| `qty` | int | 15 | Not null |
| `image` | varchar | 255 | Not null |
| `Short_desc` | varchar | 2000 | Not null |
| `description` | text | 2000 | Not null |
| `status` | tinyint | 4 | Not null |
</details>

<details>
<summary><b>Order</b></summary>

| Field | Type | Size | Constraint |
| --- | --- | --- | --- |
| `Order_id` | int | 11 | Primary key |
| `User_id` | int | 11 | Foreign key |
| `address` | varchar | 250 | Not null |
| `city` | varchar | 50 | Not null |
| `pincode` | int | 11 | Not null |
| `Payment_type` | varchar | 20 | Not null |
| `Total_price` | float | 255 | Not null |
| `Payment_status` | varchar | 20 | Not null |
| `Order_status` | int | 11 | Not null |
| `Added_on` | datetime | - | Not null |
</details>

<details>
<summary><b>Order details</b></summary>

| Field | Type | Size | Constraint |
| --- | --- | --- | --- |
| `Order_details_id` | int | 11 | Primary key |
| `Order_id` | int | 11 | Foreign key |
| `Product_id` | int | 11 | Foreign key |
| `qty` | int | 11 | Not null |
| `price` | float | - | Not null |
</details>

<details>
<summary><b>Order status</b></summary>

| Field | Type | Size | Constraint |
| --- | --- | --- | --- |
| `Order_status_id` | int | 11 | Primary key |
| `name` | varchar | 25 | Not null |
</details>

---

## Project Structure

The admin panel and storefront are built from these PHP files.

| File | Purpose |
| --- | --- |
| `connection.inc.php` | Starts the session and opens the database connection. |
| `functions.inc.php` | Shared helpers, including `get_safe_value()` for escaping input. |
| `login.php` | Admin sign-in. |
| `index.php` | Admin dashboard. |
| `categories.php` / `manage_categories.php` | List, add, edit, activate, and delete categories. |
| `product.php` / `manage_product.php` | List, add, edit, activate, and delete products. |
| `users.php` | List and delete registered users. |
| `order_master.php` | View all orders with payment and order status. |
| `search.php` | Storefront product search. |

---

## Feasibility Study

<details>
<summary><b>Read the full feasibility study</b></summary>

- **Technical:** PHP handles the interface and all application logic. MySQL stores orders, products, and user details.
- **Economic:** Development is highly economical. Customers save money and time because they no longer travel to a market to search for products.
- **Operational:** The interface is simple and attractive. Users need no special training.
- **Cultural:** Anyone can access the site with an assigned username and password. The interface is currently **English only**, with no other language option.

</details>

---

## Project Timeline

<details>
<summary><b>View the Gantt chart</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/17965bf8-82d0-43b5-85b6-f59f88e71e29" alt="Project Gantt chart" width="700">
</details>

---

## Conclusion

The project meets its design specifications and provides a user-friendly interface. All modules were tested with valid and invalid data and worked as expected.

---

## Contributing

Contributions are welcome. To propose a change:

1. **Fork** the repository.
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to your branch: `git push origin feature/your-feature`
5. Open a **pull request** describing your change.

<!-- 📌 PLACEHOLDER: link to CONTRIBUTING.md and a Code of Conduct if you add them -->

---

## License

<!-- 📌 PLACEHOLDER: choose a license (e.g. MIT) and add a LICENSE file -->
This project is licensed under the **[LICENSE TYPE]** license. See the `LICENSE` file for details.

---

## Acknowledgments

**Designed and developed by:** Deepen Ramesh Mandve, T.Y.B.Sc. (Computer Science), Semester V, 2021–2022

**Under the guidance of:** Prof. Mrs. Greta Dabre

**Institution:** A.V. College of Arts, K.M. College of Commerce, E.S.A. College of Science, Vasai Road (West), Dist. Palghar 401202, Maharashtra, affiliated with the University of Mumbai

Thanks to **Mrs. Srimathi Narayanan**, Head of the Computer Science Department, for her guidance and for the opportunity to work in the college lab. Thanks also to the Computer Science teaching staff and the laboratory staff for their support.

---

## References

- [Stack Overflow](https://stackoverflow.com)
- [W3Schools PHP Tutorial](https://www.w3schools.com/php/default.asp)
- [PHP Documentation](http://php.net/docs.php)
- [jQuery API](https://api.jquery.com)
- [Bootstrap](https://getbootstrap.com)
- [Color-Hex](https://color-hex.com)
- [GeeksforGeeks](https://geeksforgeeks.org)
- [YouTube](https://youtube.com)

<div align="center">

**If you find this project useful, please consider giving it a star.**

</div>
