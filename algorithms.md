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


##Reflection
Most of the time spent on this artifact, or rather, this portion of the artifact, was
reviewing old coursework materials from CS-300 "Data Structure and Algorithms." 
Many of the enhancements I wished to add were from this course, but I had to 
thoroughly reexamine what I had done then and how I could apply it to optimize 
this web application. 

One area that became more complex than expected was cache management. Initially, I 
focused only on improving lookup speed using unordered_map and a sorted vector with
binary search. However, I quickly realized that adding caching introduces new 
responsibilities: ensuring data consistency, handling invalidation, and preventing 
stale reads. This led me into a deeper exploration of how to manage cache state
in C++, including the use of shared mutexes and controlled rebuild logic. Previously, I had 
only encountered caching at a surface level. Working through it here gave me a much clearer 
understanding of how it can assist in performance optimizations.
