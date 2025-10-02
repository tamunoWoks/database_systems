## Database Users and Administrators
A primary goal of a database system is to retrieve information from and store new information in the database. People who work with a database can be categorized as database users or database administrators.

### Database Users and User Interfaces:
There are different types of database-system users, differentiated by the way they expect to interact with the system. Different types of user interfaces have been designed for the different types of users.

1. **Naïve Users:**  
  These are unsophisticated users who interact with the system by using predefined user interfaces, such as web or mobile applications. The typical user interface for naive users is a forms interface, where the user can fill in appropriate fields of the form. Naive users may also view read *reports* generated from the database.
As an example, consider a student, who during class registration period, wishes to register for a class by using a web interface. Such a user connects to a web application program that runs at a web server. The application first verifies the identity of the user and then allows her to access a form where she enters the desired information. The form information is sent back to the web application at the server, which then determines if there is room in the class (by retrieving information from the database) and if so adds the student information to the class roster in the database.
2. **Application Programmers:**  
  These are computer professionals who write application programs. Application programmers can choose from many tools to develop user interfaces.
3. **Sophisticated Users:**  
  These users interact with the system without writing programs. Instead, they form their requests either using a database query language or by using tools such as data analysis software. Analysts who submit queries to explore data in the database fall in this category.

### Database Administrator:
One of the main reasons for using DBMSs is to have central control of both the data and the programs that access those data. A person who has such central control over the system is called a **Database administrator (DBA)**. The functions of a DBA include:  
