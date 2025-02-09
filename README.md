# Bank System App
A C# WinForms bank system for managing accounts, transactions, and users.

## Features
- Account creation and management
- Deposit, withdrawal, and transfers
- Transaction history
- User authentication

## Technologies Used
- C# WinForms
- SQL Server
- .NET Framework 4.8

## Database Setup
### Restore from Backup (`.bak`)
1. Download `BankDB.bak` from the `Database/` folder.
2. Move it to `C:\` (or any preferred location).
3. Open **SQL Server Management Studio (SSMS)**.
4. Right-click **Databases** → **Restore Database**.
5. Select **Device** → **Browse** → Choose `BankDB.bak`.
6. Click **OK** to restore the database.
### 2️⃣ Update the Connection String in `App.config`
- Open `App.config` in the **WinForms UI project**
- Update the connection string:

#### **👉 Using SQL Server Authentication**  
```xml
<connectionStrings>
    <add name="MyDbConnection"
         connectionString="Server=YOUR_SERVER;Database=BankDB;User Id=YOUR_USERNAME;Password=YOUR_PASSWORD;"
         providerName="System.Data.SqlClient"/>
</connectionStrings>

Now, the database is ready to use!


## Installation
1. Clone the repository:
