## Database and Application Architecture
The below figure shows the architecture of a database system that runs on a centralized server machine. The figure summarizes how different types of users interact with a database, and how the different components of a database engine are connected to each other.  

![DB system structure](https://github.com/tamunoWoks/database_systems/blob/main/images/DB%20architecture.jpg "Database Architecture")

The centralized architecture shown in the figure is applicable to *shared-memory* server architectures, which have multiple CPUs and exploit parallel processing, but all the CPUs access a common shared memory.  
&nbsp;&nbsp;&nbsp;&nbsp;To scale up to even larger data volumes and even higher processing speeds, *parallel databases* are designed to run on a cluster consisting of multiple machines. Further, *distributed databases* allow data storage and query processing across multiple geographically separated machines.  

Let's now consider the architecture of applications that use databases as their backend. Database applications can be partitioned into two or three parts, as shown below:

![DB architecture tiers](https://github.com/tamunoWoks/database_systems/blob/main/images/arch%20tier.PNG "Two & Three tier DB architecture")   

Earlier-generation database applications used a **two-tier architecture**, where the application resides at the client machine, and invokes database system functionality at the server machine through query language statements.  
&nbsp;&nbsp;&nbsp;&nbsp;In contrast, modern database applications use a **three-tier architecture**, where the client machine acts as merely a front end and does not contain any direct database calls; web browsers and mobile applications are the most commonly used application clients today. The front end communicates with an **application server**. The application server, in turn, communicates with a database system to access data. The **business logic** of the application, which says what actions to carry out under what conditions, is embedded in the application server, instead of being distributed across multiple clients. Three-tier applications provide better security as well as better performance than two-tier applications.
