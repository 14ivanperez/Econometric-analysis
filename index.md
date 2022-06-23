## INDEX OF THE PROJECT
---

### 1.INTRODUCTION

The aim of the present project is to develop a theory and empirical analysis using R as a programming
language. To do so, we will answer the tasks given in the work guideline. The project structure is straight
forward: Firstly, we will answer the theory tasks assigned in the guidelines, using the knowledge that we have
acquired along the course. Secondly, using the dataset: “data_giulietti_etal.dta”, that quantifies the extent
of racial discrimination in local public services in the U.S, we will work on the tasks assinged in the project
guidelines. It is important to consider that, although there are many different ways to answer the questions
given, we have decided to answer them in such a way that the output given is the most clear to interpret.
Notice that, with the aim of distinguishing between the write-up assignment from the code we have decided
that the best idea is that the code is given in a green color. Finally, there will be a brief subsection that will
work with the monte carlo simulation.

---

### 2.THEORY TASKS

Suppose you want to quantify the extent of discrimination in public service provision in the U.S.. Your
company has collected data on email queries of citizens to public offices (libraries, police, registry), whereby
citizens were asked in a survey to provide the relevant information. In particular, the survey includes data
on 1) a person’s race – whether the person is white or belongs to a minority (Black or Latinx), and 2) data
on how many hours it takes for a public office to respond.

1.Suppose you want to estimate the effect of minority status (i.e. a dummy that equals one if a person
belongs to a minority – either Black or Latinx – and zero if the person is white) on the response time to an
email. Write down a regression equation that would allow you to estimate this effect.

2.Explain what parameter you are interested in estimating and provide an interpretation of this parameter.
We are interested in the parameter ß1, which is the slope of the regression line but also the difference in
means of two groups:

3.Discuss the random sampling assumption and the conditional independence assumption (in the lecture it
was E(u|X) = 0). Are these assumptions fulfilled in this case (explain why or why not)? Explain intuitively
the likely consequences of these assumptions (not) being fulfilled for estimating the effect of interest.

4.If you could run an experiment (regardless of ethical considerations) to estimate the effect of interest, what
would this experiment look like and why? (N.B.: the ideal experiment asked for here is different from an
experiment described further below.)

---

### 3.EMPIRICAL ANALYSIS
Libraries required
```markdown
library(gmodels)
library(tidyverse)
library(epiDisplay)
library(stargazer)
library(ggplot2)
library(haven) #for read_data
```
---

### 4. MONTE CARLO SIMULATION
<img src="images/Monte Carlo.png">



