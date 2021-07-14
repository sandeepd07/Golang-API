**Golang RESTful API using GORM and Gorilla Mux**

**Installation**

Installing the GORM, Gorilla Mux and MySQL package is fairly simple. You just need to run below three commands using GIT Bash or Putty:

go get -u github.com/gorilla/mux

go get -u github.com/jinzhu/gorm

go get -u github.com/go-sql-driver/mysql


**Run Golang RESTful API commands using GIT Bash or Putty:**

go run main.go

**Testing RESTful API methods**

**GET Method:-**

A body is never passed with a GET request to request a resource from our HTTP web servers.

GET /employees HTTP/1.1

GET /employees/name HTTP/1.1

Example:-

 URL: http://localhost:8886/employees
 
 URL: http://localhost:8886/employees/{employeename}
 
**POST Method:-**

 The POST method to send data to the server either through an asynchronous call or to execute a controller.
 
 POST /employees/data HTTP/1.1
 
Content-Type: application/json

Content-Length: xxxx 

Example:-

 URL: http://localhost:8886/employees
 
 data: {"name": "Sandeep", "age": 28, "city": "Chandigarh"}
 
 **PUT Method:-**
 
The PUT method is used to update a changeable resource and include the resource locator. Whenever we have to update a record that we have created earlier or want to create a record if it does not exist.
 
 PUT /employees/name HTTP/1.1
 
Content-Type: application/json

Content-Length: xxxx 

Example:-

  For Update Data:-
  
   URL: http://localhost:8886/employees/{employeename}
   
   data: {"age": 30}
   
   For Update Status:-
   
   URL: http://localhost:8886/employees/{employeename}/disable
   
   URL: http://localhost:8886/employees/{employeename}/enable
 
 
  **DELETE Method:-**
  
The DELETE method is always used to remove a record that is no longer required

 DELETE /employees/name HTTP/1.1
 
Example:-

 URL: http://localhost:8886/employees/{employeename}
 
 
 
 
 
 
 
