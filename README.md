# Introduction

In order to work properly and properly organize a development project, it is advisable to follow several methods.

Below, we will explain the do's and don'ts to follow in order to carry out a project in good conditions. These are tips, it's up to you to find what works best for you.

* [Task Estimation](Task-estimation)
The "Task Estimation" section will explain what a project is, what a task is and how to estimate it. We will also talk about the "SCRUM" method.
* [Coding Standards](Coding-standards)
The "Coding Standard" section will explain what coding style is through several examples and will also show you several computer language conventions.
* [Code Reviews](Code-reviews)
And finally, the "Code Reviews" section will tell you about peer programming, the different ways to do a code review and the importance of team spirit and communication within an organization.

# Task estimation

### Project estimation

**What's a project ?**

A project is defined by "an individual or collaborative enterprise that is carefully planned to achieve a particular aim".

Before defining a task, we need to define the overall project. That is, we need to think about several points that will help us to better define later the project tasks and their estimation.

The subject must be clarified to avoid confusion and misunderstanding during the project development. To ensure the project is understood by the whole team, meetings must be organized frequently during which:

- [ ] Requirements should be defined or redefined
- [ ] Long-term, mid-term and short-term objectives are then defined or redefined
- [ ] In some case, a new specific feature asked by the client may be defined
- [ ] All the tasks that need to be done are defined
- [ ] Team members that will be involved
- [ ] Project deadline might be defined

The above points are essential to plan the project the best we can. It will be important to repeat as much as possible this kind of meeting to ensure the project is going well over the time. Doing frequently meetings allow the whole team to be aware of the project advancement, if there is something new or an issue that must be treated in urge. It's also a way to ensure that everyone is working efficiently on the project priorities.

---

### Task estimation

**What's a task ?**

A task is defined by "a piece of work to be done or undertaken". So, in software progamming for example, a task could be a feature, a code review as well as writting documentation or resolving an issue.

**How to estimate a task ?**

As seen before with project estimation, several steps are needed to correctly and efficiently estimate a task duration. Some of these are also applicable to the task scope.
We will need to estimate not only the time we will need to accomplish the task but also many other things like human resources needed to handle the task, infrastructure cost, meetings needed to follow the task advancement, code reviews and many more.

**Task estimation cons and pros**

When talking about project or task estimation we obviously think about how the estimations will help the team to work efficiently and gain time on a project. But most of the time we don't take into account that taking too much time on estimations is also a lost of time in the sense that estimating could save us time thanks to a better organization but it's only worth if it's frequently done with short estimation and relatively quick decisions.

[Read more about project and task estimation](https://medium.com/globalluxsoft/time-estimation-in-software-development-a4a495c8eb6c)

# Coding standards

To begin, in order for the working group to be effective and coordinated, members need to put themselves agree on several points:
### Naming Convention

A naming convention in programming is a set of rules and coding standards for choosing the rules that will make up our source code, file identifiers and documentation. The goal is to make source code easier to read with less understanding effort to do (as if we were talking the same language and which we did not need to translate in our head). It also improves the appearance code, to avoid names that are too long or abbreviations and name identifiers that would not be understandable only by for the author of the code.

Each convention has its advantages and disadvantages depending on the languages, and each person can have their preferences. So, it is very important that the group that will work together on the same project meet upstream of the project to agree on these rules to be established. It is also necessary that the potentials groups that will work together are aware of these conventions chosen to respect them or, at least, understand code more easily when they need to read or work on it.

For example, there are several typographic standards for naming variables:
* variable_name in snake case (used in PHP, Ruby or Python)
* variableName in camelCase (found mainly in JavaScript, Java, C ++ or C #)
* VariableName in PascalCase (often used to name classes in PHP)
* variable-name in kebab-case (generally used in URLs)

[Read more](https://medium.com/better-programming/string-case-styles-camel-pascal-snake-and-kebab-case-981407998841)

These same conventions can be used to define function names or file names.

However, beware, these naming rules don't stop you from thinking. So you have to take an account other elements taken into account such as:

The meaning of the name of the variable we are going to name. It has to make sense for the oncomprehend its meaning in function.

If my function is written like this:
```
if (idx < 18) {
    var = var + 1;
    return false;
} else {
    return true;  
}
```
Or like this:
```
if (age < 18) {
    year = year + 1;
    return false;
} else {
    return true;
}

```
The last is more meaningful and is more comprehensive thanks to the name and its easily identifiable role from the first reading. The same must be done with the function names!

Then remember to respect these rules in a consistent way so that our reading of the code is not disturbed by changes without explanation.

Also be careful not to reuse the same variable name in the same class in different contexts, this provides more simplicity for understanding and maintainability.

Do not use a long name, it makes the code more difficult to read and can make the compilation more difficult with some compilers.

If you want other do's and don'ts to make sure you have a meaningful and meaningful code, I advise you to take a look [over here](https://dzone.com/articles/best-practices-variable-and)

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
### Comments Standards

**When should we comment?**
When the need or need comfort required so that other group members can understand easily function and functionality.

Remember that the comments are portions of the source code disregarded by the compiler or interpreter, because they are not necessary for the program to run. They are usually inserted in the code so that it is easy to understand and that it can be changed easily in the  future.

Developer tends to underestimate the benefits of commenting, but comment **!=** document.

Let us separate once and for all the expression document to comment.

Documenting means providing a description of its application, all of its public access points and dependencies.

Examples:

```
/*
    Comments
*/
```
Or:
```
// Comments
```
Or:
```
/**
* Comments
*/
```
Or again:
```
x = x + 1                 # Increment x
```
[Different way to comment](https://en.wikipedia.org/wiki/Comment_(computer_programming))

# Code reviews

---
### Pair programming

**What's pair programming ?**

Pair programming is a development method where two developers work on the same computer. The first, the one who writes the code is called the driver and the second, the observer, assists the driver by correcting potential errors and proposing development alternatives.

**Quality and Productivity**
Even though this practice is often abandoned by companies that think it is a waste of human resources, several studies have looked at the relative productivity of a pair of programmers versus a single programmer.
This study has proven that in terms of productivity, pair programming allows to accelerate development times especially for projects requiring a quick implementation of the solution on the market.
Pair programming allows a faster bug detection thanks to the observation of the pair programmer who realizes a code review in real time and throughout the activity. The applications created are therefore of better quality with a testing requiring less work.
The extra cost of staff (2 developers for 1) is very well compensated by the increase in development quality which allows to detect errors earlier. Indeed, the later a bug is detected, the more expensive it is to correct it.

**Communication and Team spirit**

Pair programming is a social activity that requires the ability to work in a team. It allows to develop the communication skills of the different collaborators to form a strong team spirit.
This team spirit significantly improves the well-being of the employees in their work and therefore the productivity and quality of the work provided. Indeed, many surveys have shown that more than 90% of developers prefer to program in pairs rather than alone.


**Indicators of non-performance**

Beware of non-performance indicators that can be a brake on pair programming. When training pairs, it is important to choose the employees who will work together according to the objectives of the activity.

* Silence: Pair programming requires you to program aloud and share your point of view with your partner. Persistent silence indicates a lack of collaboration.
* Disengagement: One member loses interest in the project and will go about their business.
* Deletion: When one member is more experienced than another, the novice is content to watch the expert perform the majority of the development tasks.
* Relationship problems: the two members of the pair do not get along and do not wish to work together.


Pair programming is therefore a good alternative to development alone. It allows the development of communication skills that are essential for teamwork. In companies, it is also used to quickly transfer skills.

[Read More](https://en.wikipedia.org/wiki/Pair_programming)

---

###Checklist

**The importance of checklists**

Checklists, in support of development and organization tools, are an essential tool for project monitoring and task completion. They allow you to note all the important points and discuss / carry out on the project during one day for example.

**Checklists for code reviews**

It is important to address this point in the coding review section because this tool can also be used for code reviews.
You can write down all the points to be discussed, the important things to check. Once a task is done, just check the corresponding box. It's also a tool that will free space in our memory and allow us to concentrate on the essential tasks in the work. In fact, instead of keeping in the corner of our head all the tasks we have to do, we write them down as we think about them and thus free up space in our brain to concentrate at best.

**Checklists Tools**

There are a large number of tools for making checklists called ToDoApps. On a smartphone or computer, it is up to you to choose the tool that suits you best.

Here is a non-exhaustive list of several applications:

* Any.do
* Todoist
* Microsoft To-do
* Google Task

**To go further**

It is possible with some tools like Trello or Github project to go further.
These two tools allow you to create action lists more detailed than a simple checklist. You can create lists and detail the checklist, comment on it, assign people to the task. Several other options are available that you can discover by testing the application and choose the one that suits you.
In the case of Trello and Github Project, you can also automate tasks related to git commits. For example, when the task number (which is called a ticket) is quoted in a commit, the task is checked.
