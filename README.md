
# 🛍️ ShopSharp – ASP.NET Core Web Shop

## 📋 Overview

**ShopSharp** is a full-stack e-commerce web application built with **ASP.NET Core MVC** and **Entity Framework Core**. The project simulates an online shop where users can browse products, add items to a cart, place orders, and manage accounts. Admins can manage product inventory and view user orders.

---

## 🚀 Features

### 👤 User Features
- User registration, login, and logout
- Role-based access (Customer / Admin)
- Product browsing by category
- Add to cart / Remove from cart
- Checkout and place order
- View past orders

### 🛠️ Admin Features
- Product management (Add, Edit, Delete)
- Category management
- View all orders from users

---

## 🧱 Technologies Used

| Layer            | Stack / Tool                  |
|------------------|-------------------------------|
| Frontend         | Razor Views, Bootstrap 5      |
| Backend          | ASP.NET Core MVC              |
| ORM              | Entity Framework Core         |
| Database         | SQL Server                    |
| Authentication   | ASP.NET Core Identity         |
| Dependency Mgmt  | NuGet                         |
| Version Control  | Git, GitHub                   |

---

## ⚙️ Project Structure

```
ShopSharp/
├── Controllers/         # MVC Controllers
├── Models/              # Data models (EF Core)
├── Views/               # Razor views (UI)
├── Data/                # Database context and seed data
├── wwwroot/             # Static files (CSS, JS)
├── appsettings.json     # Configuration
└── Program.cs           # App entry point
```

---

## 📦 Database Setup

1. Configure your connection string in `appsettings.json`:
   ```json
   "ConnectionStrings": {
     "DefaultConnection": "Server=.;Database=ShopSharpDB;Trusted_Connection=True;"
   }
   ```

2. Apply migrations and create the database:
   ```bash
   dotnet ef database update
   ```

---

## 🛡️ Authentication & Authorization

- Integrated **ASP.NET Core Identity**
- Roles: `Admin`, `Customer`
- Admin users have access to the product management panel
- Customers can place orders and view their order history

---

## ▶️ How to Run the App

1. Clone the repository:
   ```bash
   git clone https://github.com/Martinesko/CSharp-WEB-Application-Shop.git
   cd CSharp-WEB-Application-Shop
   ```

2. Restore dependencies:
   ```bash
   dotnet restore
   ```

3. Build and run:
   ```bash
   dotnet run
   ```

4. Visit the app at:  
   `https://localhost:5001` or `http://localhost:5000`

---

## 🧪 Test Users

You can modify the `DbInitializer.cs` or seeding logic to automatically create admin and customer test accounts with predefined credentials.

---

## 📚 Future Improvements (Optional)

- Add payment gateway integration (Stripe or PayPal)
- Product search and filtering
- User profile management
- Order status tracking
- Image upload for products

---

## 🧑‍💻 Author

**Martin Anev**  
[GitHub Repository](https://github.com/Martinesko/CSharp-WEB-Application-Shop)
