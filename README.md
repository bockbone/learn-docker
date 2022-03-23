# Learn Docker

## Command lists

  1. List all the running container.

     `docker ps`
     
  2. Run container

      `docker run -p 8080:80 -d wordpress`
      
      | Syntax      | Description |
      | ----------- | ----------- |
      | 8080        | Port        |
      | 80          | Container port        |
      | wordpress          | Container image        |
  
  3. Stop container based on ID.
     
     `docker stop [id]`
  
  4. Run the stopped container
  
      `docker start [id]`
     
  5. Show help

      `docker ps --help`
      
  6. Show all containers including the stopped container
  
      `docker ps -a`
