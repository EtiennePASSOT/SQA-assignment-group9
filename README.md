# Introduction

# Task estimation

# Coding standards

# Code reviews

---
### Pair programming

**What's pair programming ?**

Pair programming is a development method where two developers code on the same computer. The first, the one who writes the code is called the driver and the second observer assists the driver by correcting potential errors and proposing development alternatives.

**Quality and Productivity**
Even though this practice is often abandoned by companies that think it is a waste of human resources, several studies have looked at the relative productivity of a pair of programmers versus a single programmer.
This study has proven that in terms of productivity, pair programming allows to accelerate development times especially for projects requiring a quick implementation of the solution on the market.
Pair programming allows a faster bug detection thanks to the observation of the pair programmer who realizes a code review in real time and throughout the activity. The applications created are therefore of better quality with a testing requiring less work.
The extra cost of staff (2 developers for 1) is very well compensated by the increase in development quality which allows to detect errors earlier. Indeed, the later a bug is detected, the more expensive it is to correct it.

**Communication and Team spirit**

Pair programming is a social activity that requires the ability to work in a team. It allows to develop the communication skills of the different collaborators to form a strong team spirit.
This team spirit significantly improves the well-being of the employees in their work and therefore the productivity and quality of the work provided. Indeed, many surveys have shown that more than 90% of developers prefer to program in pairs rather than alone.


**Indicators of non-performance**

Beware of non-performance indicators that can be a brake on au pair programming. When training pairs, it is important to choose the employees who will work together according to the objectives of the activity.

* Silence: Pair programming requires you to program aloud and share your point of view with your partner. Persistent silence indicates a lack of collaboration.
* Disengagement: One member loses interest in the project and goes about his or her business.
* Deletion: When one member is more experienced than another, the novice is content to watch the expert perform the majority of the development tasks.
* Relationship problems: the two members of the pair do not get along and do not wish to work together.


Pair programming is therefore a good alternative to development alone. It allows the development of communication skills that are essential for teamwork. In companies, it is also used to quickly transfer skills.

[Read More](https://en.wikipedia.org/wiki/Pair_programming)

---
### Continuous integration

**What's continuous integration?**

Continous integration could be defined as a set of pratices in programming to ensure that the overall project is not impacted by a piece of code or changes pushed by someone from the developpers team.

**Continuous integegration goals**

The general purpose of continuous integration is to have unit tests on each part of the project that will be passed at each push on a branch to ensure that it will not "break" another part of the project. It may be used in a pull request for example, if the tests are all passed, then it can be merge if the reviewers aggreed on the code proposed. It is a way to ensure that developpers are coding something effectively by thinking about it before and not just pushing something working but mostly not adding a bug that will be issued later.

In general, it's only a part of a whole pipeline including several steps such as pull request and deployement

**Deployment pipeline**

Deployment pipeline is a very good practice but not used enough in practice in many companies not specialized in software development because it needs to allocate time to construct an effective pipeline as well as human resources and the companies give priority to the product development rather than the production pipeline.

[Read more about deployment pipeline](https://medium.com/the-making-of-whereby/what-is-a-deployment-pipeline-and-how-it-helps-software-development-teams-6cb29917ceea)

---

### Integration tools

As said above, continuous integration is an important practice in software development and nowadays there are many tools that can be used to easily setup the integration part in your project such as:

* TravisCI
* CircleCI
* Jenkins
* ...

Most of them could be easily integrated with GitHub, GitLab etc. in order to as mentionned before, create a pull request with a merge restriction until all unit tests are passing.

But, continuous integration is only a part of the pipeline, other tools are available to get more information about the code tested such as coverage tools.

[Example of integration tools](https://code-maze.com/top-8-continuous-integration-tools/)

---