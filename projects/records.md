---
layout: project
type: project
image: images/records.png
title: Record Database
permalink: projects/records
# All dates must be YYYY-MM-DD format!
date: 2018-04-30
labels:
  - C
  - C++

summary: A program which allows the user to read and write records to a database. Written in both C and C++.
---

This program allows the user to create, remove, and print records on the database. Records contain name, address, and an account number. The records are stored in a database in numerical order by its account number. No records can have the same account number. When adding a record with an already existing account number the account number will be incremented to the next available account number. When exiting the program, the records added/deleted will be updated in the database.

In this project, I gained deeper knowledge on how data is stored in memory and the deeper level of programming that java hides/takes care of. In a project where you have a lot of objects, it is critical in C programming to understand how memory is stored and how to retrieve data from the correct memory access.

<h2>Code</h2>

Record objects where stored in a singly linked list. Here is a the properties of a Record

<h3>Record</h3>
```
struct record
{
    int                accountno;
    char               name[25];
    char               address[80];
    struct record*     next;
};

void addRecord (struct record **, int, char [ ],char [ ]);
int printRecord (struct record *, int);
void printAllRecords(struct record *);
int deleteRecord(struct record **, int);
int readfile(struct record **, char []);
void writefile(struct record *, char []);
```
