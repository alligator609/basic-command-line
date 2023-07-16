# Run in watch mode 
```dotnet watch run // to watch changes ```
# Add database migrations
```dotnet ef migrations add AddBlogCreatedTimestamp ```
# Update database and get all the migrations into DB 
```dotnet ef database update ```
# Add Initial Migrations
```dotnet ef migrations add InitialCreate ```
# Drop database 
```dotnet ef database drop ```
# Remove last migrations
```dotnet ef migrations remove  ```
#  Using multiple context types
``` dotnet ef migrations add InitialCreate --context BlogContext --output-dir Migrations/SqlServerMigrations ```
``` dotnet ef migrations add InitialCreate --context SqliteBlogContext --output-dir Migrations/SqliteMigrations ```
