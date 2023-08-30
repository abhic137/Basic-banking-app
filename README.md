# Basic-banking-app
A basic banking app which uses docker to host a webpage using nodejs and its in memory database NeDB to access the data.
# instructions
```
cd Basic-banking-app/banking-app
```
```
docker build -t banking-app .
```
```
docker run -p 3000:3000 banking-app

```
go to browser
```
http://localhost:3000/
```
demo login credentials are
account: ```123456```
password: ```password123```
