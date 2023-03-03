#### Go languange folder structure ####

1. You can place the readme text here, like setup steps of the project, or any other information about the project that you think would be helpful for other developers/user

2. Create ".env" file, where we will keep all environment related constants, like database username, password, secret key of jwt if any, etc

3. Create the "main.go" file in root. this wi;; serve as the project/web-server entry point

4. Create a "Makefile" this will contain some basic commands to run the project

5. Create these folders:
  1. Controllers: contains controller that eccepts a request and call a particular service to process it

  2. Service: contains service that has the logic for doing all the process like manupulating DB and giving back the desired result
  
  3. Models: contains the struct for storing data in DB or fetching data from DB
  
  4. DB: keep your DB related operations here, these can be used in services to fetch/update/insert/delete data from DB
      **** Place DB connection file as well inside this folder
  5. Routes: Keep all your routes here and pass the name of controller
  6. Config: keep all your configuration things here like, fetching variables from .env file, or even db config can be placed here.
  7. Constants: Keep all constants here, can also categories then in separate files
  8. Utils: Keep commonly used functions here like capitalising first letter, etc


So, here we are ready with one of the best folder structure for a web-server development in golang there are mant weays to do it, but I follow this for a small project
