## Pro ASP.NET Core 3: Develop Cloud-Ready Web Applications Using MVC, Blazor, and Razor Pages
### Author: Adam Freeman

### Resetting the Database
> dotnet ef database drop --force --context StoreDbContext

> dotnet ef database update --context StoreDbContext

### Add Identity EntityFrameworkCore package to do Authentication & Authorization
> dotnet add package Microsoft.AspNetCore.Identity.EntityFrameworkCore --version 3.1.0

### Creating and Applying the Database Migration for Identity
> dotnet ef migrations add Initial --context AppIdentityDbContext

> dotnet ef database update --context AppIdentityDbContext

> dotnet ef database drop --force --context AppIdentityDbContext

### Publish ASP.NET Core application
> dotnet publish -c Release

## Build docker containers and Run its
> docker-compose build

> docker-compose up