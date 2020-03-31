# Introduction

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

### SCRUM method

**What's SCRUM method ?**

Scrum is an agile method dedicated to "project management". This management method, or rather this Project Management Framework, aims to improve the productivity of your team.
This method includes several roles that the whole team must play and it's very helpful to the task estimation.

### SCRUM method roles

**SCRUM Master**

- Ensures that Scrum's principles and values are respected.
- Facilitates communication within the team.
- Seeks to improve the productivity and know-how of his team.

**The team**

- No definite role: architect, developer, tester.
- All team members bring their know-how to accomplish the tasks.
- Sizes from 6 to 10 people in general and up to 200 people in particular.

**Product Owner**

- Business expert, defines functional specifications
- Prioritizes the features to be developed or corrected
- Validates the developed functionalities
- Plays the role of the customer

### Sprints

The Scrum life cycle is punctuated by iterations of a few weeks, the sprints.

### Product backlog

The initial requirements repository is established and prioritized with the customer. It constitutes what is known as the product backlog. It does not necessarily have to contain all the functionalities expected from the beginning of the project, it will evolve during the project in parallel with the customer's needs.

### User Story

The features described are called User Stories and are described using the terminology used by the client.

A User Story or Story usually contains the following information :

- [ID] a unique identifier
- [Name] a short name (between 2 and 10 words), describing the functionality expected by the customer (e.g. Export / Import Standard Sales Item). The name should be clear enough for team members and the Product Owner to understand what the function is. The name must not introduce ambiguities.
- [Importance] an integer that sets the priority of the Stories. The priority of a story can be changed during the course of the project.
- [Estimate] The amount of work required to develop, test, and validate this functionality. The unit of measure can be an ideal number of days (days 100% dedicated to the functionality) or a number of points. Estimates are made on a relative basis by comparing the estimates of completed stories with the story to be estimated.
- [Demo] A relatively simple test (e.g. export an object in XML then delete it from the database, import it from XML, at the end the object must be in the database). This test is a validation test.
- [Notes] any other information: clarifications, documentary references

### Sprint planning meeting

Before each sprint, we organize a planning meeting, the sprint planning meeting. This planning meeting selects from the product backlog the most priority requirements for the customer. They will be developed, tested and delivered to the customer at the end of the sprint. They constitute the sprint backlog, a sub-set of the product backlog.

### The scrimmage

During the sprint, a progress meeting (about 15 min) is held every day with all team members to ensure that the sprint objectives will be met, this is the Scrum. Each day, after the Scrum meeting, the Scrum Master maintains a chart called the sprint burndown chart. This chart gives a very good view of what has been done and the pace of the team's work. It also makes it possible to anticipate whether all the stories in the Sprint Backlog will be completed at the end of the iteration or not.

This meeting has not only a purely informative purpose, but also to stimulate the team spirit and the level of commitment of each team member to the project. During the meeting each team member should speak and present mainly the following things:

- What I did yesterday and any problems I encountered...
- What I'm going to do today
- Am I having difficulty continuing my work.
- By doing this exercise daily each team member is aware of what his or her colleagues are doing and can coordinate their work and help or be helped in case of difficulties.

The Scrum Meeting is not a meeting in which problems are solved, but only identified and expressed. The role of the Scrum Master is to provide solutions or to delegate to another team member the resolution of problems raised during the Scrum Meeting. Following this meeting, the Scrum Master updates the burndown chart.
At the end of a sprint, the client is given a demonstration of the latest developments, the Sprint Review Meeting. It is also an opportunity to make a review of the team's performance and to find points for improvement.

Because of its values, Scrum advocates adaptability, under the effect of the experience acquired and the specificities of the project, which brings it closer to the Toyota production method. Visibility, to evaluate the results of the process. Inspection, to verify deviations from the initial objective.

[Read more about SCRUM Method](https://en.wikipedia.org/wiki/Scrum_(software_development))

# Coding standards
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
