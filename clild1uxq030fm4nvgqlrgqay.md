---
title: "Mastering the basics: What is Data Engineering"
seoTitle: "Unleashing Data's Potential: Demystifying Data Engineering | Get Start"
seoDescription: "Discover the crucial role of data engineers in creating interfaces & mechanisms for efficient data flow and access. Learn how they set up & operate systems."
datePublished: Wed Jun 07 2023 07:00:39 GMT+0000 (Coordinated Universal Time)
cuid: clild1uxq030fm4nvgqlrgqay
slug: mastering-the-basics-what-is-data-engineering
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1686037542615/a5f9d65c-e997-43a8-a4cf-0643006d6564.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1686037243143/006a9094-4a59-4e79-a991-00d97b859a06.png
tags: data, data-engineering, data-engineer

---

In my last issue, I introduced you to the concept of data engineering, today I am going to be delving a bit deeper into the nuances of data engineering definition(s).

## What is "data engineering," really?

If you google the definition of a data engineer, you get a plethora of results defining who and what a data engineer is and what it is they do. To give some more context, let us take a couple of definitions from industry experts:

Alexsoft's definition of data engineering is "*a set of operations aimed at creating interfaces and mechanisms for the flow and access of information. It takes dedicated specialists—data engineers— to maintain data so that it remains available and usable by others. In short, data engineers set up and operate the organization’s data infrastructure, preparing it for further analysis by data analysts and scientists*"

Lewis Gavin, in his book " *What is Data Engineering?*" states that "*Data engineering is the movement, manipulation, and management of data*."

Jesse Anderson's definition gives a more elaborate definition of data engineering, dividing it into two types. Type 1 is SQL-focused data engineering, where the work and primary storage of data is in relational databases. All of the data processing is done with SQL (Structured Query Language) or a SQL-based language, and an ETL (Extract, Transform, Load) tool does this data processing. Type 2 data engineering defines big-data-focused data engineering. The work and primary storage of the data are in big-data technologies such as Hadoop, HBase, and Cassandra, with the data processing being implemented by frameworks such as MapReduce and Spark.

## **What is SQL?**

SQL is an acronym that stands for ***Structured Query Language.*** It is a programming language for storing and processing information in a relational database. A relational database stores information in tabular form, with rows and columns representing different data attributes and the various relationships between the data values. You can use SQL statements to store, update, remove, search, and retrieve information from the database. You can also use SQL to maintain and optimize database performance.

## **How does SQL work?**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686034958884/5383995a-874a-4f61-8f7c-09623b105c9d.png align="center")

Structured query language (SQL) implementation involves a server machine that processes the database queries and returns the results. The SQL process goes through several software components, including the following.

1. ### **Parser**
    

The parser starts by tokenizing, or replacing, some of the words in the SQL statement with special symbols. It then checks the statement for the following:

a. *Correctness*

The parser verifies that the SQL statement conforms to SQL semantics, or rules, that ensure the correctness of the query statement. For example, the parser checks if the SQL command ends with a semi-colon. If the semi-colon is missing, the parser returns an error.

#### b. Authorization

The parser also validates that the user running the query has the necessary authorization to manipulate the respective data. For example, only admin users might have the right to delete data.

1. ### **Relational engine**
    

The relational engine, or query processor, creates a plan for retrieving, writing, or updating the corresponding data most effectively. For example, it checks for similar queries, reuses previous data manipulation methods, or creates a new one. It writes the plan in an intermediate-level representation of the SQL statement called byte code. Relational databases use byte code to efficiently perform database searches and modifications.

1. ### **Storage engine**
    

The storage engine, or database engine, is the software component that processes the byte code and runs the intended SQL statement. It reads and stores the data in the database files on physical disk storage. Upon completion, the storage engine returns the result to the requesting application.

## What, then, is ETL?

ETL stands for extract, transform, and load. It is the process of combining data from multiple sources into a large, central repository called a data warehouse. ETL uses a set of business rules to clean and organize raw data and prepare it for storage, data analytics, and machine learning (ML)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686035850695/e0ebac0c-5649-4f59-a48a-92745e1a581e.png align="center")

## **Conclusion**

***Data engineering*** is the development, implementation, and maintenance of systems and processes that take raw data and produce high-quality, consistent information that supports downstream use cases, such as analysis and machine learning

A ***data engineer*** is an individual who manages the data engineering lifecycle, starting with fetching data from source systems and ending with serving data for use cases such as analysis and machine learning! A Data Engineer usually focuses on the middle of the data cycle. However, their work is meaningful only in light of the entire cycle.

![](https://cdn.shortpixel.ai/spai/w_567+q_lossy+ret_img+to_webp/https://www.elderresearch.com/wp-content/uploads/2020/11/image-130.png align="center")

Follow me on my next edition of #DataEngineeringFundamentals where we discuss the Data Engineering lIfecycle.

Have a great day!