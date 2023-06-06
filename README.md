# Crud_Operation_App_Nimap_Task
# Output
# FrontPage 
![Front Page](https://github.com/vedusai/Crud_Operation_App_Nimap_Task/assets/70750862/14598309-c744-4189-884a-a353ffce0f41)
# Create Page
![create](https://github.com/vedusai/Crud_Operation_App_Nimap_Task/assets/70750862/2c1f77cd-4bee-4c6c-bf79-bcbb820072ca)
# Edit Page
![Edit product Page](https://github.com/vedusai/Crud_Operation_App_Nimap_Task/assets/70750862/0233f941-808a-4a09-b943-88393a71879d)
# Details
![Dtails](https://github.com/vedusai/Crud_Operation_App_Nimap_Task/assets/70750862/0ad27bbe-e3e2-47ab-87bb-89cc91b578ec)
# Delete
![Delete](https://github.com/vedusai/Crud_Operation_App_Nimap_Task/assets/70750862/1e7dee74-34ac-4698-9a82-e756bbb5fa08)
# Database
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
