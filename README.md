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

## API Manager Endpoints:
![Screenshot (29)](https://user-images.githubusercontent.com/84228144/189864338-c40f77bc-c986-4f54-99a1-3cf20537de72.png)
![Screenshot (30)](https://user-images.githubusercontent.com/84228144/189864346-98dbc20c-675d-4674-9feb-f87cc19ec790.png)
![Screenshot (31)](https://user-images.githubusercontent.com/84228144/189864354-74429dee-d16f-4300-8cee-9648b8bdf8c0.png)
![Screenshot (32)](https://user-images.githubusercontent.com/84228144/189864356-293a1ac1-b191-455e-ac2d-dd1e6fce9713.png)
![Screenshot (33)](https://user-images.githubusercontent.com/84228144/189864357-53f7a5cb-92be-4ccf-a499-b98c3eba2e11.png)
![Screenshot (34)](https://user-images.githubusercontent.com/84228144/189864359-28741b0e-b1cd-4a35-9dc8-85069e2efcb0.png)
![Screenshot (35)](https://user-images.githubusercontent.com/84228144/189864361-85122a54-ca51-46bc-8408-dce90261da46.png)
![Screenshot (36)](https://user-images.githubusercontent.com/84228144/189864364-6c2f765c-755f-4e66-b422-b2572d598197.png)
![Screenshot (37)](https://user-images.githubusercontent.com/84228144/189864367-02c98dd9-d3c1-4b88-b190-01b8371ccd4d.png)
![Screenshot (38)](https://user-images.githubusercontent.com/84228144/189864373-8f61785f-172a-451a-aae0-386e17bdf8cb.png)
![Screenshot (39)](https://user-images.githubusercontent.com/84228144/189864375-f687f746-865a-463f-a948-5a89b9b48c30.png)
![Screenshot (40)](https://user-images.githubusercontent.com/84228144/189864376-347ec8ba-b764-49fc-9241-543593a65efb.png)
![Screenshot (41)](https://user-images.githubusercontent.com/84228144/189864378-e8de3e89-c484-43a3-9596-76e511d055a7.png)
![Screenshot (42)](https://user-images.githubusercontent.com/84228144/189864382-69f3c998-dfa2-4bc3-8cfe-7dba28db521b.png)
![Screenshot (43)](https://user-images.githubusercontent.com/84228144/189864388-9799e3d8-1f81-419b-b1b3-d260620ec27f.png)
![Screenshot (44)](https://user-images.githubusercontent.com/84228144/189864391-ded9dbf8-bf87-4161-97a9-31f8446bb765.png)
![Screenshot (45)](https://user-images.githubusercontent.com/84228144/189864396-862f5e0f-b505-4d8b-a908-26e6e809ccad.png)
![Screenshot (46)](https://user-images.githubusercontent.com/84228144/189864402-5857e26e-fd1c-4ccc-a00a-4315f7d16b62.png)
![Screenshot (47)](https://user-images.githubusercontent.com/84228144/189864403-c2225985-f049-49d5-9150-7a96083d20ce.png)

