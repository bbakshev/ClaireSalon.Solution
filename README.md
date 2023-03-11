# Eau Claire's Salon

#### By: Brishna Bakshev

## Technologies Used

* C#
* Razor HTML
* VS Code
* .Net 6
* MySQL
* Entity Framework Core 6
* CSS

## Description
This web application adds hair stylist employees and their specialties to a database through a form. It then allows adding clients through a form to each stylist and saving the information to a database. The user can then view the list of stylists and their clients. The user can also delete stylists and clients from the database.

### Setup Instructions

#### You Will Need: 

* A code editor, such as [VS Code](https://code.visualstudio.com/)
* [Git](https://github.com/) installed
* [Install .Net 6 SDK:](https://www.learnhowtoprogram.com/c-and-net/getting-started-with-c/installing-c-and-net)

#### Install MySQL Workbench:
* Follow the MySqlWorkbench installation instructions [here](https://www.mysql.com/products/workbench/), open MySql Workbench and select the Local 3306 server. Then select the "Administration" tab and click on "Data Import/Restore".
* In Import Options select "Import from Self-Contained File" and click the "..." button to navigate to the file ending in ".sql" in the top level of this repository.
* Under the "Default Schema to be Imported to" select "New..." and enter schema name of your choice. Click "Start Import" in the bottom right.
* Confirm the import was successful by clicking on the "Schemas" tab and seeing the schema you created listed.

#### Preliminary Project Set-up:
1. Clone or download this repository to your machine.
      i. Open Terminal (not including the dollar symbol):
```sh
  $ cd Desktop
  $ git clone https://github.com/bbakshev/HairSalon.Solution.git
  $ cd HairSalon.Solution
```
2. Navigate to the local directory (YourPath/HairSolution.Solution/HairSalon) and create a new file "appsettings.json".
3. Open the file in VS Code and add:
  ```
  {
    "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=[YOUR-DB-NAME];uid=[YOUR-USER-HERE];pwd=[YOUR-PASSWORD-HERE];"
    }
  }
  ```

**IMPORTANT:** Be sure to replace your username, password, and name of your database for the fields [YOUR-USER-HERE], [YOUR-PASSWORD-HERE], AND [YOUR-DB-NAME].

4. Create a .gitignore file and add "appsettings.json", "bin", and "obj" to the ignored file list.  
5. Open your shell (e.g., Terminal or GitBash) and add your .gitignore file and commit it before adding any other files. 
6. Navigate to this project's production directory called "HairSalon". 
3. In the command line, run the command `dotnet run` to compile and execute the console application. Optionally, you can run `dotnet build` to compile this console app without running it.
5. Run `dotnet watch run` in the command line to start the project in development mode with a watcher.
6. Open the browser to _https://localhost:5001_. If you cannot access localhost:5001 it is likely because you have not configured a .NET developer security certificate for HTTPS. To learn about this, review this lesson: [Redirecting to HTTPS and Issuing a Security Certificate](https://www.learnhowtoprogram.com/c-and-net/basic-web-applications/redirecting-to-https-and-issuing-a-security-certificate).

## Known Bugs

No known bugs.

## License
Enjoy the site! If you have questions or suggestions for fixing the code, please contact me!

[MIT](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt)

Copyright (c) 2023 Brishna Bakshev