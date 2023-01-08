# PostgresPreparation - Running locally


Assumptions 
1- Docker desktop is installed // you have docker in your local machine.
2- Run docker image to have the postgres container up and running using the below command:
Command: docker run --name $postgrescontainer -e POSTGRES_USER=$myusername -e POSTGRES_PASSWORD=$mypassword -p 5432:5432 -d postgres
Example: docker run --name postgrescontainer -e POSTGRES_USER=myusername -e POSTGRES_PASSWORD=mypassword -p 5432:5432 -d postgres
3- Run the following command to get inside the PSQL container:
Command: docker exec -it $postgrescontainer psql -U $myusername
Example: docker exec -it postgrescontainer psql -U myusername

Note: all $vars shall be replaced with your preferred values.

