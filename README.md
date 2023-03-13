# cass-information-system

Welcome to the cass information system github repository.

This application contains a web api written in .NET 7(C#) and a angular application. 

To run the application there are three steps you need to perform.

1: If you are using dotnet cli, go to the the project "cass-information-system\CassInformationSystemApi". And execute this command: "dotnet run". And if you are using visual studio, open the solution file using visual studio and then in the top bar click on the run button and change the selected option to "http" and then run the application.

2: Microsoft Sql Server is used for database functionality. You will have to set up the database to run the project succesfully. 
  ConnectionString that I used for my local development envoirenment is :   <br>
    - "Server=.;Database=CassDB;Trusted_Connection=True;Encrypt=False".  <br>
  Note: You can change the connection string according to your system by going into the appsettings.json file and change the default connection string.
        Also make sure that you make database CassDB in the root of Databases folder of SQLServer localhost instance.

3: Now go to the clientapp and execute these commands:
   - npm i / npm install
   - npm start
   Note: Make sure the node version is 16.10.0 and you had angular installed in your system.
   
Note: The Web Api should run on "http://localhost:5072/" and angular application on "http://localhost:4200/". If the appilcation URLs are different from these then applications might not connect with each other, in that case you will have to update the envoirnements/environment.ts in angular app and CORS section in appsettings.json in .NET application accordingly.

You can go to "http://localhost:5072/Swagger/index.html" to view the endpoints.
