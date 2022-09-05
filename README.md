# CMPG323-Project-2---30586453

![image](https://user-images.githubusercontent.com/84228144/188483008-6ec558ff-a0cd-4a83-b9d8-ddf3679dbb89.png)


## About the Project:
This is a Web API project that works together with a database called ConnectedOffice. This datase is a SQL Server database that is hosted on Azure. The database has three tables, namely; Categories, Devices, and Zone. 

This API is fundamentally an IoT Device Management System keeps track of the whereabouts of all IoT devices deployed by the organisation. Depending on the type of organisation, different categories of devices are used. Each IoT device is initially categorised and registered. Then, IoT devices are deployed throughout the organisation's buildings in predefined zones. Administrators can view all IoT devices, update their properties, add new devices and move them to other zones.  

## Security:
The API is secured in the sense not everyone has access to it right away. You must register an account in order to use the API to access and manipulate database data. This is a token based secure system. The server on which the database is hosted on is also secured, and those details are not accessible to everyone.

## Usage:
Upon accessing the API, the user must register an account. Then the user may proceed to login. The user should request a token when accessing tables and manipulating data contained in those tables.
