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

This Enhancement follows guidelines for the "Employ strategies for building collaborative environments" outcome by using clear, defined CRUD methods with adequately descriptive naming. Furthermore, it encapsulated the CRUD logic from the database logic, which enhances modularity and simplifies maintainence. Lastly, error messaging is distinct enough to be easily interpretable for developers to understand what errors are being thrown and for what. 

The "Design, develop, and deliver professional-quality oral, written, and visual communications" outcome is met by in-line comments throughout the code, along with narratives such as this one that aims to explicitly communicate what changes were made to the application. Also, as mentioned earlier, I stuck to descriptive naming practices for other hypothetical developers to easily understand what is happening during code execution. 

In order to satisfy the course outcome, "Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards" I made the intentional decision to convert the Python module into C++ for further enhancements using C++ libraries. This enhancement is the first piece of the overhaul I ultimately aimed for the web application. The major tradeoff I had to consider was weighing the simplicity of Python with the more controllable language of C++. However, I deemed the lighter-weight language and its ability to define memory usage as a natural enhancement of converting to C++.

The primary outcome I aimed to meet with this enhancement was: "Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions." I had to utilize not only built-in C++ libraries, but also external libraries such as CMake, which I integrated into vcpkg. I also had to integrate mongocxx and bsoncxx for the use of the MongoDB database. After much time debugging compilation errors, which were largely due to getting these tools to work correctly, the end result was a foundation for the algorithms and data structures enhancement that followed.

The "Develop a security mindset that anticipates adversarial exploits in software architecture and designs" was primarily met through my decision to implement exception and error handling as I converted the code. By adding proper handling, I reduced undefined behavior and was able to create exception throws that were named and defined. This 



## Screenshots

UPDATED CRUD operations:

<img width="844" height="248" alt="Screenshot 2026-02-21 105207" src="https://github.com/user-attachments/assets/05a04d8d-230d-4ce2-94e3-317a837d7d93" />
<img width="847" height="319" alt="Screenshot 2026-02-21 105243" src="https://github.com/user-attachments/assets/f016bd7d-d844-4dc4-90da-30266222ecc3" />
<img width="846" height="458" alt="Screenshot 2026-02-21 105259" src="https://github.com/user-attachments/assets/007c2555-653d-4272-8e3c-a34adc4ff290" />
<img width="852" height="307" alt="Screenshot 2026-02-21 105313" src="https://github.com/user-attachments/assets/6719f704-8f7c-44bd-bf8e-c20c76ba4a83" />

Example or Error Throwing (For Empty Filter)

<img width="787" height="52" alt="image" src="https://github.com/user-attachments/assets/bd7ab74f-9c5f-4946-96e6-27012313d00a" />


## Performance Enhancement


## Source Code Repository
The full source code, including the original implementation and the enhanced version with indexing and binary search optimizations, can be viewed here:

[View Software Engineering Enhancement Repository](https://github.com/TheScottMoore/CS499-Software-Engineering-Enhancement)
