# Stock Trading System
The application is a stock trading platform where users can buy and sell stocks

## Project Structure
```
Project\src\main
└───java
│    └───com.stock.trading
│    │    └───controllers
│    │    └───dtos
│    │    └───models
│    │    └───repository
│    │    └───services
│    │    │ StockTradingSystemApplication.java

└───resources
└───webapp
│    └───css
│    └───images   
│    └───js
│    └───logo   
│    └───WEB-INF 
│ pom.xml

```
## Initial Setup
Pre Requisites:
1. Install Docker for desktop and download postgres image
2. Install pgAdmin to work with Postgres DB.
3. Install IntelliJ or Eclipse to run Spring Application
4. Have Minimum of Java 1.8 setup in your system

## How to Run
###Docker
1. Open Docker desktop
2. Run the following command in cmd/GIT cmd to run docker container for PostGres server instance
    ```
   docker run --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=password -d postgres
   ```

###PgAdmin
1. Open PgAdmin and create database server using the UI under Dashboard with following details:
```
Server Name: stock-trading-db
Host Name/ Address: localhost
Port: 5432
Username: postgres
Password: password
```
2. Create a DB within the server with the following details:
```
Name: stock-trading-db
```

###Intellij
1. Download the source code
2. Open Intellij
3. Open the code as maven project and let the IDE create indexes and initialize the Spring project
4. Run src\main\java\com\stock\trading\StockTradingSystemApplication.java as Spring boot application (Run button next to Class name)


###Browser
1. Open Chrome, Edge browsers and incognito instances to login as different users.
2. Type "localhost:8080" in address bar
3. Login:
- Login as admin using the below credentials:
```
   Admin:
   user: admin
   password: admin
```
- To Login as user, create a user using email and password. Login with those credentials.
```
   For user:
   user: $user_email
   password: $user_password

```

4. As admin, Create stock using the UI provided in the menu at the top.
5. As the new user explore the features of the app.

###Features
- Admin
1. Can see the current stock market.
2. Can see details of each stock present in the marketplace.
3. Can add a new stock.
4. Can manage market settings.
5. Can see list of users.
- User:
1. Can see the current stock market
2. Can see details of each stock.
3. Can view the stocks they own.
4. Can sell the stocks by creating limit order.
5. Can buy stocks from market or limit order.
6. Can see the transaction history
7. Can add money to their wallet



## Author
Name: Sundaravadivel Chandrasekaran Ponmudi \
Email ID: sundaravadivelcp@gmail.com \
Demo Video: [Demo Video](https://youtu.be/iXIrzWYfaTg)