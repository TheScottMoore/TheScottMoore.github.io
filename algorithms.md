---
title: Algorithms and Data Structures
---

{% include nav.html %}

# Algorithms Enhancement

## Overview
This artifact was originally developed for CS-340: Client/Server Development. 
The application was written in Python and connected to a MongoDB database 
to manage records for trained rescue animals sourced from animal shelters.
The original purpose of this project within CS-340 was to demonstrate the
ability to link the front-end and back-end components into a working web
application. 

## Justification
This full-stack application was a great choice as an artifact to demonstrate
my skill in utilizing advanced sorting algorithms, knowledge of when to use
which algorithm (In this case, Sorted-Vector/Binary Search and Hash Indexing) 
to use to optimize for query and sort time complexity. The enhancements I 
applied to the original application are not so noticeable currently, as the 
database is relatively small, but would be much more significant if the application
were to scale. Optimizing for time complexity will shorten query times and use fewer 
resources to accomplish the task. Not only was time complexity optimization enhanced
through sorting algorithms, but with cache management was also demonstrated throughout.


## Reflection
Most of the time spent on this artifact, or rather, this portion of the artifact,
reviewing old coursework materials from CS-300 "Data Structure and Algorithms." 
Many of the enhancements I wished to add were from this course, but I had to 
thoroughly reexamine what I had done then and how I could apply it to optimize 
this web application. 

One paticular area that became complex was cache management. Initially, I 
focused only on improving lookup speed using a sorted vector with binary search. 
However, I learned that adding caching introduces new abilities such as ensuring data 
consistency, handling invalidation, and preventing stale reads. This led me into a 
rabbit hole of how to manage cache state in C++, including the use of shared mutexes
and controlled rebuild logic. Previously, I had only encountered caching at skin level. 
Working through it here and actually succeeding in getting it to work, makes me 
feel far more comfortable optimizing in C++.

This artifact enhancement meets the "Design and evaluate computing solutions" as it
successfully implemented algorithms, data structures, and cache management to 
optimize the original artifact. By doing this, the application no longer just 
queries the database, but uses hash indexing and binary search, which were deemed
to be the most appropriate tools to enhance this artifact.

This artifact enhancement also meets the "Demonstrate an ability to use well-founded
and innovative techniques, skills, and tools in computing practices" outcome because
I had to implement the MongoDB C++ driver and configure CMake, which led to the need
to debug many a compiler issue to get it to run. The open-ended nature of this assignment
required the falling back on learned best practices and researching new tools.

I would say this enhancement doesn't really work with the "Design, develop, and deliver 
professional-quality oral, written, and visual communications" outcome by itself, because
beside its in-line notations, doesn't really communicate much to an audience. 

The enhancement was designed be used with the original dashboard and database, it
does meet "Employ strategies for building collaborative environments." While this artifact 
is not inherently collaborative, preserving compatibility with the original dashboard 
allows it to integrate into shared systems and workflows. By preserving compatibility, the 
work here is useful to anyone familiar with the original application.

Lastly, this enhancement alone doesn't fully address the security mindset outcome. Even 
though I changed the application from using the hard-coded credentials like the original 
used, I did not focus on utilizing too many of the secure-coding best practices.

<img width="481" height="229" alt="image" src="https://github.com/user-attachments/assets/a7e35d79-a292-478e-951d-fc423044311c" />

Successfully compiles and executes using hash indexing and binary search range query



