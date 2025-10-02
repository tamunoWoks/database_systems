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
One of the main reasons for using DBMSs is to have central control of both the data and the programs that access those data. A person who has such central control over the system is called a **Database administrator (DBA)**, and the functions of a DBA include:  
  - **Schema definition:** The DBA creates the original database schema by executing a set of data definition statements in the DDL.
  - **Storage structure and access-method definition:** The DBA may specify some parameters pertaining to the physical organization of the data and the indices to be created.
  - **Schema and physical-organization modification:** The DBA carries out changes to the schema and physical organization to reflect the changing needs of the organization, or to alter the physical organization to improve performance.
  - **Granting of authorization for data access:** By granting different types of authorization, the database administrator can regulate which parts of the database various users can access. The authorization information is kept in a special system structure that the database system consults whenever a user tries to access the data in the system.
  - **Routine maintenance:** Examples of the database administrator's routine maintenance activities are:
    - Periodically backing up the database onto remote servers, to prevent loss of data in case of disasters such as flooding.
    - Ensuring that enough free disk space is available for normal operations, and upgrading disk space as required.
    - Monitoring jobs running on the database and ensuring that performance is not degraded by very expensive tasks submitted by some users.

Enterprises are increasingly outsourcing the storage and management of their data. Rather than maintaining in-house systems and expertise, enterprises may store their data in "cloud" services that host data for various clients in multiple, widely distributed server farms. Data are delivered to users via web-based services. Other enterprises are outsourcing not only the storage of their data but also whole applications. In such cases, termed "*software as a service*," the vendor not only stores the data for an enterprise but also runs (and maintains) the application software. These trends result in significant savings in costs, but they create new issues not only in responsibility for security breaches, but also in data ownership, particularly in cases where a government requests access to data.
&nbsp;&nbsp;&nbsp;&nbsp;The huge influence of data and data analytics in daily life has made the management of data a frequent aspect of the news. There is an unresolved tradeoff between an individual's right of privacy and society's need to know. Various national governments have put regulations on privacy in place. High-profile security breaches have created a public awareness of the challenges in cybersecurity and the risks of storing data.
