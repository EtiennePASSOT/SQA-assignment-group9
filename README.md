# Introduction

# Task estimation

# Coding standards

To begin, in order for the working group to be effective and coordinated, members need to put themselves agree on several points:
### Naming Convention

A naming convention in programming is a set of rules and coding standards for choosing the rules that will make up our source code, file identifiers and documentation. The goal is to make source code easier to read with less understanding effort to do (as if we were talking the same language and which we did not need to translate in our head). It also improves the appearance code, to avoid names that are too long or abbreviations and name identifiers that would not be understandable than for the author of the code.
Each convention has its advantages and disadvantages depending on the languages, and each person can have their preferences. So, it is very important that the group that will work together on the same project meet upstream of the project to agree on these rules to be established. It is also necessary that the potentials groups that will work together are aware of these conventions chosen to respect them or, at least, understand code more easily when they need to read or work on it.

For example, there are several typographic standards for naming variables:
* variable_name in snake case (used in PHP, Ruby or Python)
* variableName in camelCase (found mainly in JavaScript, Java, C ++ or C #)
* VariableName in PascalCase (often used to name classes in PHP)
* variable-name in kebab-case (generally used in URLs)

[Read more](https://medium.com/better-programming/string-case-styles-camel-pascal-snake-and-kebab-case-981407998841)

---
### Coding Style

**What's coding style ?**
The coding style is a set of rules used in programming when writing source code. These rules allow to have symmetrical source codes no matter the developer and therefore a standard code readable and understandable by all. It is also a good way to avoid errors when writing code.

One of the most important things of coding style is indentation. It allows to quickly identify the different code blocks, functions and methods.

For example :
```
if (hours < 24 && minutes < 60 && seconds < 60)
    return true;
else
    return false;
```

```
if  ( hours   < 24
&& minutes < 60
&& seconds < 60)
return true;
else
return false;

```

These two blocks of code make it possible to perform exactly the same action and yet the first block is much simpler to read and it is also easier to identify the different conditions (and therefore to identify potential errors).


Another very important point is spacing. Like the indentation, it mainly allows a better reading and understanding of the code.

For example :
```
int i=0;
for(;i<10;i++){
    printf("%d",i+(i*2));
}
```


```
int i = 0;
for (; i < 10; i++) {
    printf("%d", i + (i * 2));
}
```

These two blocks of code perform exactly the same action except that the second block is much easier to read than the first.

> Be careful not to put spaces unnecessarily everywhere which can deteriorate the simplicity of reading and no longer in the language standards.

The last essential point of the coding style are the characters ```{ }``` which are used in almost all programming languages. They allow to create condition blocks or loops as seen above. These characters are also important in terms of their placement in the code.

For example :
```
if (hours < 24 && minutes < 60 && seconds < 60) {
    return true;
} else {
    return false;
}
```

```
if (hours < 24 && minutes < 60 && seconds < 60)
{
    return true;
}
else
{
    return false;
}
```
Here, reading is quite simple in both cases, but good practice in certain languages prefers to use one or the other.

In conclusion, it is important to respect the code standards provided by the different languages. When it is possible to write in different ways, development teams must choose the writing that suits them in order to have a uniform code.


---
### Languages Convention

The world of computer development is formed by many languages, frameworks and development tools. All languages have best practices and writing conventions.
It is very important to follow the conventions set up by the community of the language / framework in question. This allows a symmetry of code between all programs developed with the same language. It is also a way to read and understand anyone's code quickly.
We will see the code conventions for one programming language and one framework.
These are examples and there are conventions for all languages.

Each language has its own conventions but some are common to all languages :
* Follow the DRY Principle (Don't Repeat Yourself)
* Limit line length
* Keep the code simple


##### Convention in C language

To write code following best practices, you must first learn about naming conventions.
For example in the C language :

Variables and functions are written in [camelCase](https://en.wikipedia.org/wiki/Camel_case) :
```
int nbPeoples;
openFile();
```

In C language, the files are organized this way :
```
  /* macros ============================================================== */
  /* constants =========================================================== */
  /* types =============================================================== */
  /* structures ========================================================== */
  /* private variables =================================================== */
  /* private functions =================================================== */
  /* internal public functions =========================================== */
  /* entry points ======================================================== */
  /* public variables ==================================================== */
```

[Read more](https://www.topcoder.com/coding-best-practices/)

##### Convention in Symfony Framework

The symfony framework also follows the writing of functions, methods and variables in [camelCase](https://en.wikipedia.org/wiki/Camel_case)
For the configuration of parameters and twig template variables, use the [snake_case](https://en.wikipedia.org/wiki/Snake_case)
For naming PHP namespaces and classes, use the [UpperCamelCase](https://en.wikipedia.org/wiki/Camel_case)


The naming conventions used are different depending on what is needed, which makes it possible to quickly identify variables and functions of PHP classes for example.

Here is a non-exhaustive list of Symfony conventions
* Add a single space after each comma delimiter;
* Add a single space around binary operators (==, &&, ...), with the exception of the concatenation (.) operator;
* Use return null; when a function explicitly returns null values and use return; when the function returns void values;
* Declare public methods first, then protected ones and finally private ones. The exceptions to this rule are the class constructor and the setUp() and tearDown() methods of PHPUnit tests, which must always be the first methods to increase readability;


[Read more](https://symfony.com/doc/current/contributing/code/standards.html)

---


# Code reviews
