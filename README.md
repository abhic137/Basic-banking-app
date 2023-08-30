# Basic-banking-app
A basic banking app which uses docker to host a webpage using nodejs and its in memory database NeDB to access the data.
# instructions
```
cd Basic-banking-app/banking-app
```
```
sudo docker build -t banking-app network --host .
```
```
sudo docker-compose up -d
```
```or```
```
sudo docker run -p 3000:3000 banking-app

```
go to browser
```
http://localhost:3000/
```
demo login credentials are
account: ```123456```
password: ```password123```

If you want to add account and password we have to insert the data into the database (do this before building the docker file and running it)
```
cd backend
sudo nano server.js
```
and add your credentials ike this
```// Insert valid account data into the database
db.insert(
  [
    { accountNumber: '123456', password: 'password123', balance: 1000 },
    { accountNumber: '987654', password: 'letmein', balance: 500 }
  ],```
