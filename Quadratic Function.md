---
title: "Quadratic Function"
author: "Lev Savolsky"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```
## This is a markdown file
### Introduction

Hello, my name is Lev and I chose to describe you how to draw a graph of a simple quadratic function using **`plot()`** function in R as my Coursera project.

### Drawing

Firstly, we need to create a new R script, in R Studio - File -> New File -> R Script, or we can use Ctrl+Shift+N on Windows. In this file we'll need to write a function **`Draw`**, for example:
```{r}
Draw <- function(x, y) {
    plot(x, y, type="l", xlab="x-axis", ylab="y-axis", 
         main="Quadratic function")
}
```
As parameters for our function we take coordinates on the x-axis - **`x`** and a quadratic function - **`y`**. To draw our graphic we use function **`plot()`** here, as parameters we give our x and y variables, *type = "l"* stands for type of demonstration - lines, in *xlab* and *ylab* we write what should be shown next to the x-axis and y-axis, *main* parameter is the heading.

After we wrote our fuction we should run it first, then we go to the console in the bottom left of the screen, we initialize aour x and y variables like that:
```{r}
x <- (-10:10)
y <- 3*x^2 + 2*x + 4
```
We initialized *x* variable as a vector of integers to have a set of coordinates on our graph.

Now, finally, we can call our **`Draw(x, y)`** function and draw a graph of *3\**x^2 + 2\**x + 4* by writing:
```{r}
Draw(x, y)
```


## *Thank you for reading and good luck on the next Data Science courses!*

---
