# Lab 5: Javacc

In this lab, the lab builds on the example calculator provided by Infoworld.
Start by reading their article: <https://www.infoworld.com/article/2076269/build-your-own-languages-with-javacc.html>
In this article they show how to set up a language to support math operating for addition, subtraction, multiplication, and division.
Expressions can even have parenthesis and include precedence.

First understand you must generate the compiler code by running `maven compile` (or `maven generate-sources`).
This can be done in your IDE.

The calculator has been modified to build the code in a package.
Otherwise this has been copied from the website.
A set of JUnits have been added to confirm the system is working.

## Your tasks

You must modify the calculator to include five functions.

* Modulo (`%`)
* Exponent (`^`)
* Minimum (`min(a,b)`)
* Maximum (`min(a,b)`)
* Round (`round(value,decimals)`)

Each function should have an accompanying test.
Write JUnit test for each of your new functions.
Make sure to maintain precedence.

## Executing the program

The project uses Apache Maven to compile and run the project.
This is all done through the command line.

Compile project to byte code and output to the target directory:

```shell
mvn compile
```

Remove target directory.

```shell
mvn clean
```
