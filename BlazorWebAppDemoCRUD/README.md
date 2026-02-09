# EF Core Setup — Data Layer Foundation

This branch introduces the complete Entity Framework Core foundation for the Blazor Web App. It includes the data model, database context, connection string configuration, and prepares the project for migrations and CRUD operations.

---

## What Was Added in This Branch

### 1. Installed EF Core Packages
The following NuGet packages were added to enable database access, SQL Server support, and migration tooling:

- `Microsoft.EntityFrameworkCore`
- `Microsoft.EntityFrameworkCore.SqlServer`
- `Microsoft.EntityFrameworkCore.Tools`

---

### 2. Added the `Product` Entity
A new `Product` class was created in:
Models/Product.cs

This defines the core data structure for CRUD operations.

---

### 3. Added the `AppDbContext`
A new EF Core database context was added in:


This context exposes the `Products` DbSet and configures EF Core for the application.

---

### 4. Added the Connection String
A SQL Server LocalDB connection string was added to:

appsettings.json
This enables local development and testing without external dependencies.

---

### 5. Registered EF Core in Program.cs
The `AppDbContext` was registered with the dependency injection container, enabling EF Core throughout the application.

---

## Next Step in This Branch

Run the first EF Core migration to generate the database and create the `Products` table:

Add-Migration InitialCreate Update-Database


---

## Why This Branch Matters

This branch establishes the entire data layer for the application. All future CRUD features will build on this foundation. Keeping this work isolated in its own branch ensures:

- clean commit history  
- easy code review  
- clear curriculum chapters  
- reproducible steps for learners  

