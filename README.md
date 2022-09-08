# CMPG323-Project-2---30586453

![image](https://user-images.githubusercontent.com/84228144/188483008-6ec558ff-a0cd-4a83-b9d8-ddf3679dbb89.png)


## About the Project:
This is a Web API project that works together with a database called ConnectedOffice. This datase is a SQL Server database that is hosted on Azure. The database has three tables, namely; Categories, Devices, and Zone. 

This API is fundamentally an IoT Device Management System keeps track of the whereabouts of all IoT devices deployed by the organisation. Depending on the type of organisation, different categories of devices are used. Each IoT device is initially categorised and registered. Then, IoT devices are deployed throughout the organisation's buildings in predefined zones. Administrators can view all IoT devices, update their properties, add new devices and move them to other zones.  

## Creation of the API
### Azure database
Started off with creating an account on Azure and created a resource group, under which I added an SQL database and hosted my database there. I then added tables to the database via Sql Server Management Studio (SSMS). 

![image](https://user-images.githubusercontent.com/84228144/188954455-9c9160fd-10b9-426a-9c1b-2e6dfefdff0a.png)

### API creation
I used visual studio to create the web API. Added controllers that will support the manipulation of tables in the database that is hosted on azure server. Thereafter I implemented security on the API so that no unauthorized user can get access to the API functionality.

### Hosting the API
I created an API Management Service on azure so that I could be able to work with it there. I then published the API via Visual Studio, and pulled it from the Azure side. 

![image](https://user-images.githubusercontent.com/84228144/188955239-3eea68ed-1e7b-4681-9870-b87450945dc7.png)


## Security:
The API is secured in the sense not everyone has access to it right away. You must register an account in order to use the API to access and manipulate database data. This is a token based secure system. The server on which the database is hosted on is also secured, and those details are not accessible to everyone.

## Usage:
Upon accessing the API, the user must register an account. Then the user may proceed to login. The user should request a token when accessing tables and manipulating data contained in those tables. The account that should be registered is the admin one because it is the only one that is authorized to access the tables.

### Registering an account:
The user must register an admin user because it is the only role that is authorized to access he tables and table manipulation.

### Logging in:
The user must click on the login button and insert the newly registered credentials.After logging in the user will receive the token. That token must be saved as will be used to access the tables since this system uses a tokeen based security.

### Working with tables:
Before doing anything the user must click on the lock logo to get authorization to access the tables. A window will appear where they will need to type "Bearer" followed by the token they received when logging in. Thereafter the user can use the POST, GET, PUSH and more funtionalities of the system.
