# Products List Page (READ)

This branch introduces the first UI milestone for the Blazor CRUD application.  
It implements the **Products List page**, which retrieves data from the EF Core backend and displays it in a clean, interactive table.

## ✔️ Features Implemented
- New `Products.razor` page
- Injected `AppDbContext` or ProductService (depending on architecture)
- Asynchronous data loading with `OnInitializedAsync`
- Table layout for displaying product data
- Navigation links for Create, Edit, and Delete (placeholders for now)

## ✔️ Why This Matters
This is the first point where the backend and UI connect.  
Learners can now see real database data rendered in the Blazor UI.

## ✔️ Next Steps
- Implement Create Product page
- Implement Edit Product page
- Implement Delete confirmation
- Add validation and UX polish