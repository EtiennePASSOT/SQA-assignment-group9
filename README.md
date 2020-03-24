# Introduction

# Task estimation

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

---



# Code reviews
