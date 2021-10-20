# BucketServer
Small API with SQLite database that saves notes for an iOS appliction called Bucket list. This project is done using Vapor 4, and has all CRUD operations implemented using the /tasks and /tasks/<ID> endpoints.
  
## Endpoints
### Creating a task 
  POST "(localhost)/tasks"\
  Header "Content-Type: application/json"\
  Body: 
 >  {"objective": "My first tasks"} \
 ### Reading all tasks
 GET "(localhost)/tasks"\
 Header "Content-Type: application/json" \
 
 ### Updating a tasks 
  POST "(localhost)/tasks/(id)" \
  Header "Content-Type: application/json" \
  Body: 
 >  {"objective": "Writing to vapor and updated objective here "} \
  
 ### Delete a tasks
  DELETE "(localhost)/tasks/(id)" \
  Header "Content-Type: application/json" \
  
  
    
