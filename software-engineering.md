---
title: Software Engineering
---

{% include nav.html %}

# Software Engineering Enhancement

## Overview
This artifact was originally developed for CS-340: Client/Server Development. The application was written in Python and connected to a MongoDB database to manage records for trained rescue animals sourced from animal shelters. The original purpose of this project within CS-340 was to demonstrate the ability to link the front-end and back-end components into a working web application.

## Justification
For this Enhancement, I aimed to convert the Python data transfer layer into C++. I also took the opportunity to add error/exception handling to further enhance this module. This took some effort as Python and C++ are significantly different languages,as Python is an interpreted language while C++ directly compiles into machine code. However, this was an excellent choice for my software development enhancement as it would set me up for my following two enhancements and allow me to utilize C++ libraries for sorting algorithms and specifically cache memory management, which Python does not directly allow.  

## Reflection
Setting up my environment and determining which libraries I needed was the most time-consuming and challenging aspect of this conversion. The code within the original file is relatively straightforward and simple to understand; therefore, rewriting it in C++ was not overly complicated as long as I had the right dependencies to continue using the database and dash system. Including basic exception handling was important to me to implement now, as it would be included in subsequent enhancements.



## Screenshots

Successful data migration to a new SQLite Database using a Python script
<img width="802" height="109" alt="Screenshot 2026-02-07 145514" src="https://github.com/user-attachments/assets/173a2379-7499-41ad-b2a5-17327084c427" />


Screenshot of the dashboard system after the database change
<img width="1264" height="890" alt="Screenshot 2026-02-07 171607" src="https://github.com/user-attachments/assets/16bf2577-8824-4a0b-84e6-8d9f64d4c97b" />



## Performance Enhancement
This enhancement was primarily about converting a non-schema database into a schema database. The benefits of this are that it ensures complete and uniform data, simplifying maintainability and query optimization. Another thing to note is that the SQLite database significantly reduces the number of dependencies compared to MongoDB which simplifies portability and reduces complexity as well as eliminates the need for external servers so that local deployments are much simpler. Admittedly, this enhancement would not be ideal for an application that aims to optimize for cloud-based and distributed systems, in which the original MongoDB database structure would actually be the better choice.

## Source Code Repository
The full source code, including the original implementation and the enhanced version with indexing and binary search optimizations, can be viewed here:

[View Software Engineering Enhancement Repository](https://github.com/TheScottMoore/CS499-Software-Engineering-Enhancement)
