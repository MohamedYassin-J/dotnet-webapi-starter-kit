## Setting Startup Projects
Before applying the database migrations, ensure that you have set the correct startup projects:
##### Web API:
Ensure that the ***"Host"*** project is set as the single startup project.

##### WebAssembly:
Ensure that the ***"Client"*** project is  set as the single startup project.

Now, you can proceed to apply the database migrations:
## Database Migrations
Before running the application, make sure to apply the database migrations. Navigate to the `src\Migrators\Migrators.MSSQL` directory and use the following commands:
```powershell
PM> Update-Database -Context ApplicationDbContext
PM> Update-Database -Context TenantDbContext
```

## Default Super Admin Client Credentials
The default super admin client credentials are as follows:
```json
{
    "email": "admin@root.com",
    "password": "123Pa$$word!"
}
```

## Hangfire Credentials
To access Hangfire dashboard, you'll need the following credentials:
```json
{
  "User": "Admin",
  "Password": "S3(r3tP@55w0rd"
}
```