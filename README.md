# Crud_Operation_App_Nimap_Task
# Output
# FrontPage 
![Front Page](https://github.com/vedusai/Crud_Operation_App_Nimap_Task/assets/70750862/14598309-c744-4189-884a-a353ffce0f41)

    CREATE TABLE Category (
       CategoryId INT PRIMARY KEY Identity,
       CategoryName VARCHAR(255)
       );

	   CREATE TABLE Product (
       ProductId INT PRIMARY KEY Identity,
       ProductName VARCHAR(50),
	   CategoryName VARCHAR(50) Not Null,
       CategoryId INT ,
       FOREIGN KEY (CategoryId) REFERENCES Category(CategoryId)
       );
