# ASP.NET-WebAPI-CRUDExample

*How to create basic CRUD Operation in Web API?
1️⃣ Create a new ASP.NET Core Web API project
2️⃣ Install NuGet packages:
      Microsoft.EntityFrameworkCore.SqlServer
      Microsoft.EntityFrameworkCore.Tools
3️⃣ Create Models folder → Add model class (e.g., Employee.cs)
4️⃣ Create Data folder → Add DbContext class and DbSet for model
5️⃣ Create database and from properties of DB copy connection string and Add connection string in appsettings.json
6️⃣ Register DbContext and connection string in Program.cs
7️⃣ Create the database using EF Core Migrations means run following commands in package manager console:
      dotnet ef migrations add Initial
      dotnet ef database update
8️⃣ Create Service Contract folder → Add Interface for CRUD operations
9️⃣ Create Service folder → Add Implementation class (inject DbContext, implement CRUD)
🔟 Register Service Interface + Implementation in Program.cs
1️⃣1️⃣ Create Controllers folder → Add API controller, inject service, implement CRUD endpoints
1️⃣2️⃣ Test CRUD operations using Postman
