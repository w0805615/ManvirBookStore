﻿2023-03-02
1505
Assignmnet#2 in-class in the lab
3.1(out of support)
individual Account authentication
No Razor
Reviewed Areas folder

1506 - in Startup.cs on line 33
removed options for the default identity:
options => options.SignIn.RequireConfirmedAccount = true

1510
Tested the app...everything OK
Actions Items:
Modify the navigation
Update the Copyright ...from static to dynamic
make repository -public

1513
Upadted the Welcome message
tested
Reviewed the Route pattern in startup.cs

Created Github repository

2023-03-03
1515
Test the app...

1525
Created a README.md file in the github and pulled it to the VS2019

2023-03-09
1414
Choosed a Darkly theme from the bootswatch.com
Renamed the older bootstrap file 
Added new bootstrap.css in 
Lib > bootstrap > dist > css > bootstrap.css

Made changes in _Layout.cshtml
renamed bootstrap.min.css to bootstrap.css
nav class from navbar-light to navbar-dark to bg-primary
Line 23 remove text dark
added text-white-50 bg-primary to the footer

Now in _LoginPartial.cshtml
removed text-dark

1429
Tested the app 
It worked!

1451
Added a live date in the footer of the layout.cshtml page

1455
Modified a navigation 
at the place of home nav I added a Books link
which is currently empty because I havent created the database yet.

1505
Almost Done
just need to make my repository public from private

1539
Added additonal css and scripts links in the layout.cshtml

1903
Dropdown worked
some of the attributes were missing that is why it didn't show up 
But now everthing looks fine!
Moving on to the next step!

1519
Added new projects

2023-03-23
1502

Continue!
Moved the Data Folder and paste to .DataAccess project(Deleted the original)

1521
Install NuGet package
- Identity.EntityFrameworkCore

Modified namespace
Deleted all default Class1.cs in all projects

Moved Models to the ManvirBooks.Models project and deleted the original

1537
Added project References
Renamed Models folders to View Models
Updated the HomeController.cs

Done for now!
Continue Later!

1816
the error: The type or namespace name 'ApplicationDbContext' could not be found
Solved!

Successfully Run the Application

Updated Files:
Error.cshtml
startup.cs
HomeController.cs

1822
Created new class in Utility project and added project References to utility project as well as Data Access
Added new class Customer to the Areas folder
Updated Routes in Startup.cs
pattern: "{area:Customer}/{controller=Home}/{action=Index}/{id?}");

ERROR!! page is not responding

Solved the ERROR:
endpoints.MapAreaControllerRoute(
        name: "defaultArea",
        areaName: "Customer",
        pattern: "{controller=Home}/{action=Index}/{id?}");

1857 Everything looks GOOD!

1904
Added a new Admin area in Areas
Added the proper view files and delete the Data and Models folder
Deleted the controllers folder

Assignment 2 Part 1 DONE!

2023-03-24
1505
Assignment 2 Part 2 
Start!

Updated the Database name in appsettings.json
Database=ManvirBookStore

Added migrations
add-migration AddDefaultIdentityMigration (this is a wrong default project)
New migration file name= ManvirBookStore.DataAccess

MIGRATION FILES:
20230324192450_AddDefaultIdentityMigration.cs
20230327220200_AddCategoryToDb.cs

1551
ERROR!
update-database
Build failed

2023-03-27
1803
Error Solved!
by updating NuGet Packages

Checked the tables in SQl Server ObjectExplorer

1806
Added new class Category class in Models, Modified
Once again Run the migration and updated the database
Reviewed Updataed database in SQl Server ObjectExplorer

Everything Look fine!

1821
Added New folders in ManvirBooks.DataAccess
Repository > IRepository > IRepository.cs
Added New class : Repository.cs
Modifeid both the classes with the given instructions

2023-03-29
1315
Created the individual repositories for category:
CategoryRepository.cs
ICategoryRepository.cs
Modified 
Resolved Errors!


2023-03-30
1703
Added new Interface in IRepository folder
-ISP_Call.cs
installed Nuget packages for Dapper

1730
Implemented new class - SP_Call.cs in the Repository 
Modified according to intructions
Added using statements
NO ERRORS!

RUN THE PROJECT
SUCCESSFULL!

1803
Added a new interface UnitOfWork
Modified 

1830
Modified startup.cs in the ConfigurationServices method
NO ERRORS
PROJECT RUN!


