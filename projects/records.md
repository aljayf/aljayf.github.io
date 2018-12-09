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

summary: A program which allows the user to read and write records to a database. Written in two versions; C and C++.
---

This program allows the user to create, remove, and print records on the database. Records contain name, address, and an account number. The records are stored in a database in numerical order by its account number. No records can have the same account number. When adding a record with an already existing account number the account number will be incremented to the next available account number. When exiting the program, the records added/deleted will be updated in the database.

In this project, I gained deeper knowledge on memory management. In a project where you have a lot of objects, it is critical in C programming to understand how memory is stored and how to retrieve data from the correct memory access. Dealing with pointers and using the heap presented some challenges, but it allowed me to understand how computers work. Another thing I learned was the basic C standard IO functions to read and write to files.

<h2>Code</h2>

Record objects where stored in a singly linked list. Below is the properties of a Record object.

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

<h2>Sample Output</h2>
```
1. Add a new record in the database
2. Print information about a record using the accountno as the key
3. Print all information in the database
4. Delete an existing record from the database using the accountno as the key
5. Quit the program
Type the corresponding number to perform the action
1
You have selected to add a record in the database
Enter the account number of the record to be added
1
Name: John Doe
You may now enter the address of the record.
Enter ';' at the end to finish input
Honolulu
Hawaii;
Account was successfully added
```
