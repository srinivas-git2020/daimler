# daimler
created new spring boot projets for client and resource server.
check out and import the code into IDE. Execute  mvn clean install. mvn spring-boot:run to start the application for both projects.
client application is running in 8080 port. Hit http://localhost:8080/getAuthorizationCode  
It display authorization  Details, client_id = daimler , response_type = code, redirect_uri= http://localhost:8090/getAccessToken, scope= "read" and click on GetAccessToken.
resource server is running at 8090 port and it validate above mentioned authorization details  and re-direct to resource server login page.
login id= admin, password= admin. and submit the reuest.
after providing authorization access is Accept, it will redirect to GetAccessToken jsp page and it will display access token.
