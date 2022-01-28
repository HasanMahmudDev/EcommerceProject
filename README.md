SmartShop
A Ecommerce site Made with ASP .NET Core , ASP .NET Web API & Angular

#Technologies at glance
Frontend Technologies
JavaScript
Angular
TypeScript
SignalR
Backend Technologies
ASP .NET Core Web API
ASP .NET Core
EntityFrameworkCore
SignalR
Requirement
node js
Visual Studio Code 2019
dotnet ef global tool if you don't have, using this command to install dotnet tool install --global dotnet-ef
Installation guide
Download the repository.
Open the SmartShop.DataApi project in the command prompt & write the below command.
Add migration for SmartShopDbContext - dotnet ef migrations add "SS_v0" --project ..\SmartShop.DataLib\SmartShop.DataLib.csproj --startup-project .\SmartShop.DataApi.csproj -c SmartShopDbContext
Update migration for SmartShopDbContext - dotnet ef database update "SS_v0" --project ..\SmartShop.DataLib\SmartShop.DataLib.csproj --startup-project .\SmartShop.DataApi.csproj -c SmartShopDbContext
Update migration for AppDbContext - dotnet ef database update -c AppDbContext
Open SmartShop.Web project in the command prompt and run the server on 5001 port - dotnet run --urls=http://localhost:5001
Open the SmartShop.DataApi project in the command prompt and run - dotnet run
Open the SmartShop.Web\ClientApp in the command prompt and run - npm install & then ng serve -o
