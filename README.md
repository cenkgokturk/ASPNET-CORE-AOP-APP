## Description

Basic [ASP.NET](http://asp.net/) Core Model-View-Controller app built on C# with user authentication. Furthermore, Aspect-Oriented programming was used for logging user activity and admin chec

## Necessary Programs/Libraries

Program was written in C#, therefore, a special environment for the aforementioned language is needed (Visual Studio 2019 was used for the project). User authentication is being handled by the Identity API on [ASP.NET](http://asp.net/) Core with features such as cookies and password recovery. Net Core 5.0 was used for the application and no prior version was tested. If you have an older version, libraries and APIs might result in errors. Finally, in order to store user data including first and last name, email address and password, a local SQL server is needed. SQL Server Management Studio (Version 18.8) was used to initialize a database.

## How to Install

1. Download the source code from the given GitHub repository
2. Open the program in Visual Studio
3. Make the following changes to the AOPContentConnection variable in appsettings.json file
    - Server=[Must be the name your local SQL server]
    - Database=[Pick a name for the table to hold user credentials]
4. Go to Tools → NuGet Package Manager → Package Manager Console
5. Enter the following commands separately 

    ```jsx
    Add-Migration "Initial-Create"
    Update-Database
    ```

6. Finally, to run the application, click Ctrl+F5 (Start without debugging)
7. Program will be opened in a new tab in your default browser