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
   
  7. Remove stopped container
  
      `docker rm [id]`
      
  8. Force removed running container

      `docker rm -f [id]`
      
  9. Format the text when using `docker ps`
      
      `export FORMAT="ID\t{{.ID}}\nNAME\t{{.Names}}\nIMAGE\t{{.Image}}\nPORTS\t{{.Ports}}\nCOMMAND\t{{.Command}}\nCREATED\t{{.CreatedAt}}\nSTATUS\t{{.Status}}\n"`
      
      `docker ps --format=$FORMAT`
   
  10. 
