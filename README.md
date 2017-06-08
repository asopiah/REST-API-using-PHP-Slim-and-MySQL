# REST-API-using-PHP-Slim-and-MySQL
Simple REST API in PHP and MySQL
1. Prerequisite
 
 Basic knowledge on PHP, JSON parsing and  MySQL communication is recommended.
 
 2. Slim PHP Micro Framework
 
 Rather than devolping the REST API from scratch, I have use Slim framework becoz of the following reasons:
  
  a)It supports all HTTP methods i.e GET, POST, PUT and DELETE which are necessary for a REST API
  
  b)It is a very light weight framework, clean and a beginner can easily understand the framework without much straining.
 
 c)It provides a middle layer architecture which is veryseful in filtering  requests. e.g verifying API keys
  
  Downloading Slim Framework below
    
    https://github.com/codeguy/Slim
 
 3. Downlaod and Instal and run XAMP Server (Apache, PHP and MySQL) on your machine 
    
    
    *Open http://localhost/phpmyadmin/ to verify xamp is installed and running successfully.
    
    *Open the phpmyadmin from http://localhost/phpmyadmin and execute the SQL queries in the rest_api.sql file inside the db folder. 
    
    You can alternatively import the .sql file
    

4. Install Chrome Advanced REST client (ARC) extension or PostMan extension for Testing the API
 
 
5. Testing the API


Following is the list of URL we need to test using Chrome Advanced REST client extension with possible combinations of inputs.


URL	                                                  Method	         Parameters	                        Description

http://localhost/task_manager/v1/register	        POST	   name, email, password	            User registration

http://localhost/task_manager/v1/login	          POST	   email, password	                  User login

http://localhost/task_manager/v1/tasks	          POST	   task	                              To create new task

http://localhost/task_manager/v1/tasks	          GET		                                      Fetching all tasks

http://localhost/task_manager/v1/tasks/:id	      GET		                                      Fetching single task

http://localhost/task_manager/v1/tasks/:id	      PUT		                                      Updating single task

http://localhost/task_manager/v1/tasks/:id	      DELETE	 task, status	                      Deleting single task
