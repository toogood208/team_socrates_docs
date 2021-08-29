# Package
This directory contains the base folder which houses the local data stored and other local database operations,  as well as the server-request folder which contains the API, logic and code for sending and receiving data to and from the server
## base
This folder serves as base folder for the Package directory, it contains the local_db folder
### local_db
The local_db folder stores data in the local database using shared preferences,
this enables offline access of data to the app,
data such as number, bool, string can be stored in the local_db folder.
it also manages logic related to CRUD(Create, Read, Update, Delete) operations on device storage.
#### local_db.dart
local_db.dart contains the logic for storing data on local device
### server-request
The server-request folder contains files used for sending data and receiving appropriate
response from the server.
#### get_request.dart
The get_request.dart file contains requests made to the backend
using APIs to fetch and serve data.
#### post_request.dart
The post_request.dart file contains logic and data to be sent to the server most likely for storing it, commonly used for uploading a file or submitting a web form.

