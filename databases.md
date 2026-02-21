---
title: Databases
---

{% include nav.html %}

# Databases Enhancement

## Overview
This artifact was originally developed for CS-340: Client/Server Development. The application was written in Python and connected to a MongoDB database to manage records for trained rescue animals sourced from animal shelters. The original purpose of this project within CS-340 was to demonstrate the ability to link the front-end and back-end components into a working web application.

## Justification
This full-stack application was a great choice as an artifact to demonstrate my skill in creating, transforming, migrating, and indexing databases. As I no longer had access to the original database for the original project, I had to create a fresh database using MongoDB that would work with my other code files. After accomplishing that and creating 60 documents within the database, I created a Python script to migrate and transform that data into an SQLite structured/schema-based database. Afterwards, I modified my code files to operate using the new SQLite database and successfully executed the application using the front end dashboard.

## Reflection
The most complicated portion of this part of the overall project was creating the Python script that migrated the data from the MongoDB database to the new SQLite database while also ensuring perfectly consistent formatting. Fortunately, there are a lot of examples available to create a script like this, and I was able to migrate all 60 documents to the new database without much trouble. Another significant part of the work was modifying the CRUD module to operate with the new database. This took more than just changing the name of the database referenced within the module. I also had to update the function calls and then alter the dashboard for it to continue working.

This enhancement took purposeful steps to fulfill the "Employ strategies for building collaborative environments" outcome as the migration perserved the structure, field names, and compatibility with the orignal web application. Only some small changes were needed to convert the original Python module and dashboard so utilizing the new SQLite database would be relatively painless for another developer to do so. Admittedly, much of the modularity of this web application was baked in originally by using the original Python module. After converting it to C++ in the previous categories, it still maintained much of its modularity, making it easy to maintain and update.

Although the database enhancement itself does not demonstrate much of the "Design, develop, and deliver professional-quality oral, written, and visual communications" outcome, the written narratives, such as this one, are aimed at clearly communicating what was done to enhance the artifact.

The "Design and evaluate computing solutions that solve a given problem" outcome was met within this database category by projection data transfer, implementing reusable helper functions, and preserving the compatibility with the original dashboard. The decision to take advantage of the MongoDB C++ driver and continue to use a new C++ module data access layer followed best practices for database access and functions rather than relying on raw database queries. 

Much like the last outcome, the outcome of: "Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions," was demonstrated by the decisions on how to execute my goal of converting the database while still maintaining compatibility with the front-end dash system. I used the MongoDB C++ driver, created a Python script for migration, and ensured my query builders were properly encapsulated to perserve a fully functional full-stack application that still operated the some from the end-users perspective.

The "Develop a security mindset that anticipates adversarial exploits in software architecture and designs," outcome was met as I deliberately deployed strategies to prevent attacks such as SQL Injection and removed hard-coded credentials. The original hard-coded credentials were replaced by using an environment-based configuration, which reduces the risk of compromising the credentials if the source code was revealed, and I added input validation and proper error-handling to mitigate risks of SQL Injection attacks. Together, this application, though not entirely secure as possible, is still far more difficult to attack than the original application was.

## Screenshots

Successful data migration to a new SQLite Database using a Python script
<img width="802" height="109" alt="Screenshot 2026-02-07 145514" src="https://github.com/user-attachments/assets/173a2379-7499-41ad-b2a5-17327084c427" />


Screenshot of the dashboard system after the database change
<img width="1264" height="890" alt="Screenshot 2026-02-07 171607" src="https://github.com/user-attachments/assets/16bf2577-8824-4a0b-84e6-8d9f64d4c97b" />



## Performance Enhancement


## Source Code Repository
The full source code, including the original implementation and the enhanced version with indexing and binary search optimizations, can be viewed here:

[View Database Enhancement Repository](https://github.com/TheScottMoore/CS499-Database-Enhancement)
