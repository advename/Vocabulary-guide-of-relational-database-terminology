# Relational database correct terms and why there is an inconsistency
While I was learning, in more depth, the relational database using books, tutorials, guides and articles, I've quickly got confused as there is a tremendous inconsistency in the relational database terminology.

Here an example:
- Person A: A field is the same as a column
- Person B: A field is an intersection between a column and a row

This can quickly lead to confusions when the context is not clear at the beginning of the text.

But where did this inconsistency originate from and what are the actual "correct" terms? 
That's what we will have a look at in this article.

## History
Before we can analyze the origination of the term's, we somehow have to understand some history pieces of data and relational database.

In the old days, data was stored using a *file-based system* <sup>1</sup> . A company system has a number of applications programs; each of them is designated to manipulate data files (imagine files with the `.txt` extension). Each single file contained records of data, e.g. a Client File contained records of Clients.   

In 1970, E.F. Codd introduced the world to his research paper "A Relational Model of Data for Large Shared Data Banks" <sup>2,3</sup>. In this paper and later papers, he defined what he meant by "relational". He is the inventor and father of the relational model and relational algebra <sup>4,5,6</sup> , which is closely derived from the mathematical set theory <sup>7</sup>.

In 1979, based on E.F. Codd's relational database paper, Oracle released the first commercial relational database management system (RDBMS)

## Origination
Based on history, we can continue with the three subjects file-based system, relational algebra and the relational database management system.

While working or operating with every single one of them, you need to use different terms.

**File-based system**
A group of data is stored in files. A single entry is called a record.

**Relational algebra**
The relational algebra uses operators from the set theory with additional constraints and allows “new” relations to be derived from “old” ones. Every relation has a
heading and a body: The heading is a set of attributes (whereby the term attribute I mean an
attribute-name/type-name pair), and the body is a set of tuples that conform to that
heading.

**Relational database management system**
A relational database management system consists of one or multiple tables. A table is a collection of related data held in a table format within a database. It consists of columns and rows.

## Terms comparison 
As you probably have noticed, these subjects have one thing in common, processing data. However, they are different things.

![Relational database terms](https://raw.githubusercontent.com/advename/Vocabulary-guide-of-relational-database-terminology/master/relational-database-terms-difference.jpg)

## Conclusion
Even if the valid terms are table, column and rows, educational programs, articles and many other sources are still mixing them up and that to an extent that the correctness of using them can be considered as not important. All that matters is that you communicate in a way that everyone understands. Therefore, it's important to define the terms to be used in teams to prevent confusions.


**Sources:**
1. [Chapter 1 Before the Advent of Database Systems – Database Design – 2nd Edition](https://opentextbc.ca/dbdesign01/chapter/chapter-1-before-the-advent-of-database-systems/)
2. [Relational database - Wikipedia](https://en.wikipedia.org/wiki/Relational_database)
3. [Relational algebra - Wikipedia](https://en.wikipedia.org/wiki/Relational_algebra)
4. [A relational model of data for large shared data banks](https://dl.acm.org/citation.cfm?id=362685)
5. [Relational database - Wikipedia](https://en.wikipedia.org/wiki/Relational_database)
6. [David Maier: The Theory of Relational Databases](http://web.cecs.pdx.edu/~maier/TheoryBook/TRD.html)
7. [Set theory - Wikipedia](https://en.wikipedia.org/wiki/Set_theory)

**Additional sources and inspiration:**
- [terminology - Column vs Field: have I been using these terms incorrectly? - Database Administrators Stack Exchange](https://dba.stackexchange.com/questions/65609/column-vs-field-have-i-been-using-these-terms-incorrectly)
- [terminology - What is the difference between a "record" and a "row" in SQL Server? - Database Administrators Stack Exchange](https://dba.stackexchange.com/questions/31805/what-is-the-difference-between-a-record-and-a-row-in-sql-server?noredirect=1&lq=1)
- [Relational database - Wikipedia](https://en.wikipedia.org/wiki/Relational_database)
- [Data Modeling - Conceptual, Logical, and Physical Data Models](https://www.1keydata.com/datawarehousing/data-modeling-levels.html)
- Joe celko - data & databases: concepts in practice
- C.J. Date - An introduction to database systems
- C.J. Date - The new relational database dictionary
- E.F. Codd - The relational model for database management

