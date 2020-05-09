Steps to follow 

1) Create 2 seperate code base for each microservice

2)Create controller which will call processRequest method in BC 

3) Create BC which will have processRequest method which will validate request and call DAC and map data to response object  return response to controller.

4)Create DAC which will have methods which save data to and retrieve data from JSON files. ( if Oracle DB connectivity is available you go for database operations) and return data to BC for mapping with response object.

5)Design RAML for  use attached sample  movie.raml for reference

6)Create Models ( request and response type) using RAMLS tools for .NET.  It is available in Visual studio marketplace. Download this plugin using extension manger in Visual studio.  provide your created RAML to this tool and it will create models/contracts. To access this tool right click on  your servicehost project click on Add RAML contract.

7)Use Models for request and response mapping 

8) Test your API using postman/ soap UI



