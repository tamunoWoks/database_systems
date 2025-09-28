# Database System Concepts
A **database-management system (DBMS)** is a collection of interrelated data and a set of programs to access those data. The collection of data, usually referred to as the **database**, contains information relevant to an enterprise. The primary goal of a DBMS is to provide a way to store and retrieve database information that is both convenient and efficient.  
&nbsp;&nbsp;&nbsp;&nbsp;Database systems are designed to manage large bodies of information. Management of data involves both defining structures for storage of information and providing mechanisms for the manipulation of information. In addition, the database system must ensure the safety of the information stored, despite system crashes or attempts at unauthorized access. If data are to be shared among several users, the system must avoid possible anomalous results.

### Database-System Applications
All database applications, old and new, share important common elements. The central aspect of the application is not a program performing some calculation, but rather the data themselves. Today, some of the most valuable corporations are valuable not because of their physical assets, but rather because of the information they own.  

Database systems are used to manage collections of data that:
- are highly valuable
- are relatively large, and
- are accessed by multiple users and applications, often at the same time.  

Modern database systems exploit commonalities in the structure of data to gain efficiency but also allow for weakly structured data and for data whose formats are highly variable. As a result, a database system is a large, complex software system whose task is to manage a large, complex collection of data.  

Managing complexity is challenging in any domain. Key to the management of complexity is the concept of *abstraction*.  
&nbsp;&nbsp;&nbsp;&nbsp;**Abstraction** allows a person to use a complex device or system without having to know the details of how that device or system is constructed. For a large, complex collection of data, a database system provides a simpler, abstract view of the information so that users and application programmers do not need to be aware of the underlying details of how data are stored and organized. By providing a high level of abstraction, a database system makes it possible for an enterprise to combine data of various types into a unified repository of the information needed to run the enterprise.  

Databases form an essential part not only of every enterprise but also of a large part of a person's daily activities. Although user interfaces hide details of access to a database, and most people are not even aware they are dealing with a database, accessing databases forms an essential part of almost everyone's life today.  

Broadly speaking, there are two modes in which databases are used:
  - The first mode is to support **online transaction processing**, where a large number of users use the database, with each user retrieving relatively small amounts of data, and performing small updates. This is the primary mode of use for the vast majority of users of database applications such as those that we outlined earlier.
  - The second mode is to support **data analytics**, that is, the processing of data to draw conclusions, and infer rules or decision procedures, which are then used to drive business decisions.

For example, banks need to decide whether to give a loan to a loan applicant, online advertisers need to decide which advertisement to show to a particular user. These tasks are addressed in two steps. First, data-analysis techniques attempt to automatically discover rules and patterns from data and create *predictive models*. These models take as input attributes (“features”) of individuals, and output predictions such as likelihood of paying back a loan, or clicking on an advertisement, which are then used to make the business decision.  
&nbsp;&nbsp;&nbsp;&nbsp;As another example, manufacturers and retailers need to make decisions on what items to manufacture or order in what quantities; these decisions are driven significantly by techniques for analyzing past data, and predicting trends. The cost of making wrong decisions can be very high, and organizations are therefore willing to invest a lot of money to gather or purchase required data, and build systems that can use the data to make accurate predictions.  

#### Data Mining:
The field of *data mining* combines knowledge-discovery techniques invented by artificial intelligence researchers and statistical analysts with efficient implementation techniques that enable them to be used on extremely large databases.

### Purpose of Database Systems
To understand the purpose of database systems, consider part of a university organization that, among other data, keeps information about all instructors, students, departments, and course offerings. One way to keep the information on a computer is to store it in operating-system files. To allow users to manipulate the information, the system has a number of application programs that manipulate the files, including programs to:
- Add new students, instructors, and courses.
- Register students for courses and generate class rosters.
- Assign grades to students, compute grade point averages (GPA), and generate transcripts.  

Programmers develop these application programs to meet the needs of the university, and new application programs are added to the system as the need arises. New application programs may also have to be written to handle new rules in the university. Thus, as time goes by, the system acquires more files and more application programs.  

This typical **file-processing system** is supported by a conventional operating system. The system stores permanent records in various files, and it needs different application programs to extract records from, and add records to, the appropriate files.  

Keeping organizational information in a file-processing system has a number of major disadvantages:
  - Data redundancy and inconsistency.
  - Difficulty in accessing data.
  - Data isolation.
  - Integrity problems.
  - Atomicity problems.
  - Concurrent-access anomalies.
  - Security problems.

### View of Data
A database system is a collection of interrelated data and a set of programs that allow users to access and modify these data. A major purpose of a database system is to provide users with an *abstract* view of the data. That is, the system hides certain details of how the data are stored and maintained.
