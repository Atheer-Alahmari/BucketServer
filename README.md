# BucketList Server-Side
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
  PUT "(localhost)/tasks/(id)" \
  Header "Content-Type: application/json" \
  Body: 
 >  {"objective": "Writing to vapor and updated objective here "} \
  
 ### Delete a tasks
  DELETE "(localhost)/tasks/(id)" \
  Header "Content-Type: application/json" \
  
  # Running project 
First install home brew: https://brew.sh 

Then open terminal and run  

Commands 
>	brew install vapor \
>	vapor 

When you run vapor and see a list of commands then you have successfully install vapor 

Now clone or download the repo to your desktop using GitHub desktop or whatever you prefer 
https://github.com/rodleyva/BucketServer/tree/master 

Next we’ll cd and build our project 
It’s important the project is in your desktop or the next commands won’t work 

Commands 
>	cd ~/Desktop/(name of the project folder) \
>	vapor build \
>	vapor xcode 

Then just run the project on Xcode and you will get a local server usually like 
http://127.0.0.1:8080  
 
# Errors

If you get a "vapor: Address already in use" error just do this in terminal 
 
> sudo lsof -i :8080 \
> kill {PID of the process}

Then run the project again
  
reference: https://stackoverflow.com/questions/53298296/vapor-address-already-in-use-errno-98 
  
    
