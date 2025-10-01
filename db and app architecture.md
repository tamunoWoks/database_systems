## Database and Application Architecture
The below figure shows the architecture of a database system that runs on a centralized server machine. The figure summarizes how different types of users interact with a database, and how the different components of a database engine are connected to each other.  

![DB system structure](https://github.com/tamunoWoks/database_systems/blob/main/images/DB%20architecture.jpg "Database Architecture")

The centralized architecture shown in the figure is applicable to *shared-memory* server architectures, which have multiple CPUs and exploit parallel processing, but all the CPUs access a common shared memory.  

To scaler up to even larger data volumes and even higher processing speeds, *parallel databases* are designed to run on a cluster consisting of multiple machines. Further, *distributed databases* allow data storage and query processing across multiple geographically separated machines.
