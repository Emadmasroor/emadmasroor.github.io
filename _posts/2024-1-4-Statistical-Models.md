---
layout: distill
title: Statistical Models
description: Webpage of the Course 551305 T2 2023/24
giscus_comments: false
tags: teaching maths
date: 2024-1-4



authors:
  - name: Silvio Fanzon
    url: "https://www.silviofanzon.com/"
    affiliations:
      name: University of Hull, UK
      department: Department of Mathematics
      state: United Kingdom


bibliography: teaching.bib


toc:
  - name: General Information
  - name: Questions
  - name: Key Links
  - name: Lectures Calendar
  - name: Assessment
  - name: Topics
  - name: Lectures Diary
  - name: Statistical tables
  - name: R codes
  - name: Datasets
  - name: Homework
  - name: References



---

## General Information

Welcome to the Course **Statistical Models 551305** for the BSc in Mathematics at the University of Hull, academic year 2023/24. 
This module focusses on both the technical and practical aspects of a range of linear statistical models. We will investigate how and why these models work, what the assumptions 
behind them are, and how to interpret the results. We will also implement such models using the programming language R.


- **Lecturer**: Dr Silvio Fanzon
- **Email**: [S.Fanzon@hull.ac.uk](mailto:S.Fanzon@hull.ac.uk)
- **Office**: Room 104a, Larkin Building
- **Office hours**: Wednesday 12:00-13:00
- **Canvas Page**: Click [here](https://canvas.hull.ac.uk/courses/70065)




## Questions


If you have any questions please feel free to `email me`. We will address Homework and Coursework in class. In addition, please do not hesitate to attend `office hours`.




## Key Links


All the course information will be posted on this page, as well as on [Canvas](https://canvas.hull.ac.uk/courses/70065). The links to the reference material are:

- **[Slides](https://www.silviofanzon.com/2024-Statistical-Models-Slides/)**
- **[Lectures Diary](#lectures-diary)**
- **[Homework](#homework)**




## Lectures Calendar


We have two `Lectures` and one `Tutorial` per week:


- **Lecture 1**: Wednesday 10:00-12:00 in Wilberforce Building - Lecture Room 22
- **Lecture 2**: Thursday 15:00-17:00 in Wilberforce Building - Lecture Room 10
- **Tutorial**: Thursday 11:00-12:00 in Wilberforce Building - Lecture Room 7




## Assessment


This course will be assessed as follows:


|**Type of Assessment**                | **Percentage of final grade** |
|: -----                 |: -----                        |
|  Coursework Portfolio  | 70%                           |
|  Homework              | 30%                           |



**Rules for Coursework**: 


- Coursework available on Canvas from Week 3

- We will discuss coursework exercises in class

- Coursework must be submitted on **[Canvas](https://canvas.hull.ac.uk/courses/70065)** by **14:00 on Thursday 2nd May 2024**



**Rules for Homework**:


- There will be 10 Homework papers, posted weekly on **[Canvas](https://canvas.hull.ac.uk/courses/70065)** 

- Each Homework paper is worth 14 points

- Final Homework grade computation: 
    * Sum the top 7 scores (max score 98 points)
    * Bonus 2 points will be added to the final score

- Homework papers must be submitted on **[Canvas](https://canvas.hull.ac.uk/courses/70065)** by **14:00 on Mondays**. Due dates are listed **[below](#homework)**





**How to submit assignments**:


- Submit **PDFs only** on **[Canvas](https://canvas.hull.ac.uk/courses/70065)**

- You have two options:
	* Write on tablet and submit PDF Output
	* Write on paper and **Scan in Black and White** using a **Scanner** or **Scanner App** (Tiny Scanner, Scanner Pro, ...)


**Important**: I will not mark


- Assignments submitted **outside of Canvas**
- Assignments submitted **After the Deadline**





## Topics

- Linear regression models with one or more explanatory variables
- Least squares estimation of model coefficients and their properties
- Checking the regression modelling assumptions
- Analysis of variance (ANOVA)
- Analysis of real-world datasets
- Statistical software for testing, prediction and visualisation of data





## Lectures Diary

There are **11 lectures** in this module. Links to the slides and lecture titles are below



|**Week of**| **Slides**                                                                                                   | **Title**  			            |
|: -----    |:---------      									                           | :---------                                     |
| 29 Jan    | [Lecture 1](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_1.html#/title-slide)  | An introduction to Statistics                  |  
| 5 Feb     | [Lecture 2](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_2.html#/title-slide)  | Multivariate distributions                     |
| 12 Feb    | [Lecture 3](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_3.html#/title-slide)  | Random samples                                 |
| 19 Feb    | [Lecture 4](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_4.html#/title-slide)  | Hypothesis tests in R -- Part 1                |
| 26 Feb    | [Lecture 5](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_5.html#/title-slide)  | Hypothesis tests in R -- Part 2                |
| 4 Mar     | [Lecture 6](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_6.html#/title-slide)  | Two-sample hypothesis tests                    |
| 11 Mar    | [Lecture 7](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_7.html#/title-slide)  | The chi-squared test                           |
| 18 Mar    | [Lecture 8](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_8.html#/title-slide)  | The maths of regression                        |
| 8 Apr     | [Lecture 9](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_9.html#/title-slide)  | General linear regression                      |
| 15 Apr    | [Lecture 10](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_10.html#/title-slide)| Practical regression                           |
| 22 Apr    | [Lecture 11](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_11.html#/title-slide)| Violation of regression assumptions and ANOVA  |
| 29 Apr    | Revision Week                                                                                                | Coursework submission deadline                 |
| Extra     | [Appendix](https://www.silviofanzon.com/2024-Statistical-Models-Slides/slides/lecture_12.html#/title-slide)  | More on R                                      |



## Statistical tables

- Available [here](/assets/pdf/teaching/2024-Statistical-Models/Statistics_Tables.pdf)




## R codes

| **Lecture** | **Material**                                                                                                                                                                              | 
|:------      |:------                                                                                                                                                                                    |
| Lecture 4   | [One-Sample t-test](/assets/pdf/teaching/2024-Statistical-Models/one_sample_t_test.R) 													  |
| Lecture 5   | [Variance ratio test](/assets/pdf/teaching/2024-Statistical-Models/variance_ratio_test.R)                                                                                                 |
| Lecture 6   | [Two-Sample t-test](/assets/pdf/teaching/2024-Statistical-Models/two_sample_t_test.R) \| [F-test](/assets/pdf/teaching/2024-Statistical-Models/F_test.R)  <br>   [F-test First Principles](/assets/pdf/teaching/2024-Statistical-Models/F_test_first_principles.R)    |
| Lecture 7   | [Goodness-of-fit](/assets/pdf/teaching/2024-Statistical-Models/good_fit.R) <br> [Goodness-of-fit First Principles](/assets/pdf/teaching/2024-Statistical-Models/good_fit_first_principles.R) <br> [Monte Carlo pi](/assets/pdf/teaching/2024-Statistical-Models/monte_carlo_pi.R) <br> [Monte Carlo p-value](/assets/pdf/teaching/2024-Statistical-Models/monte_carlo_p_value.R) <br> [Goodness-of-fit Contingency](/assets/pdf/teaching/2024-Statistical-Models/good_fit_contingency.R) <br> [Independence Test](/assets/pdf/teaching/2024-Statistical-Models/independence_test.R) |
| Lecture 8   | [Least-squares Solution 1](/assets/pdf/teaching/2024-Statistical-Models/least_squares_1.R) <br> [Least-squares Solution 2](/assets/pdf/teaching/2024-Statistical-Models/least_squares_2.R)   |
| Lecture 9   | [Multiple regression](/assets/pdf/teaching/2024-Statistical-Models/multiple_regression.R) <br> [R2 multiple regression](/assets/pdf/teaching/2024-Statistical-Models/R2_multiple_regression.R)|
| Lecture 10  | [Simple regression](/assets/pdf/teaching/2024-Statistical-Models/simple_regression.R) <br> [Longley regression](/assets/pdf/teaching/2024-Statistical-Models/longley_regression.R) <br> [Longley selection](/assets/pdf/teaching/2024-Statistical-Models/longley_selection.R) <br> [Galileo](/assets/pdf/teaching/2024-Statistical-Models/galileo.R) <br> [Divorces](/assets/pdf/teaching/2024-Statistical-Models/divorces.R) |
| Lecture 11  | [Residual graphs](/assets/pdf/teaching/2024-Statistical-Models/residual_graphs.R) <br> [Autocorrelation graphic tests](/assets/pdf/teaching/2024-Statistical-Models/autocorrelation_graph_tests.R) <br> [Multicollinearity](/assets/pdf/teaching/2024-Statistical-Models/multicollinearity.R) <br> [Stepwise Regression: Longley](/assets/pdf/teaching/2024-Statistical-Models/longley_stepwise.R) <br> [Stepwise Regression: Divorces](/assets/pdf/teaching/2024-Statistical-Models/divorces_stepwise.R)  <br> [Anova models](/assets/pdf/teaching/2024-Statistical-Models/anova.R)  |
| Appendix    | [2008 Crisis](/assets/pdf/teaching/2024-Statistical-Models/2008_crisis_code.R)  |


## Datasets

- [Stock-Gold prices](/assets/pdf/teaching/2024-Statistical-Models/stock_gold.txt) 
- [Longley](/assets/pdf/teaching/2024-Statistical-Models/longley.txt)
- [Fridge Sales](/assets/pdf/teaching/2024-Statistical-Models/fridge_sales.txt)
- [2008 Crisis](/assets/pdf/teaching/2024-Statistical-Models/2008_crisis.txt)
- [Family Guy](/assets/pdf/teaching/2024-Statistical-Models/family_guy.txt)



## Homework


Homework papers must be submitted on **[Canvas](https://canvas.hull.ac.uk/courses/70065) by 14:00 on Mondays**



|  **Homework #** |**Due date**   |  **Topics**                                                                                              |
|: --------       |:------------- |:---------                                                                                                |
| 1               | 5 Feb         |  Moment generating function. Poisson distribution.                                                       |
| 2               | 12 Feb        |  Poisson models for soccer                                                                               |
| 3               | 19 Feb        |  Computing the pdf of Student's t distribution                                                           |
| 4               | 26 Feb        |  t-test in R and by hand                                                                                 |
| 5               | 4 Mar         |  Cancelled. Replaced by Homework 8 now worth 28 points                                                   |
| 6               | 11 Mar        |  Chi-squared distribution and variance ratio test                                                        |
| 7               | 18 Mar        |  Properties of chi-squared and F-distribution                                                            |
| 8               | 8 Apr         |  Homework 8 is worth 28 points. Two-sample t-test and F-test. Chi-squared tests                          |
| 9               | 15 Apr        |  Simple and general linear regression                                                                    |
| 10              | 22 Apr        |  t-test and F-test for regression                                                                        |




## References


- **Slides**: Available **[here](https://www.silviofanzon.com/2024-Statistical-Models-Slides/)**


- **Main References**: The slides are self-contained and based on the books

	* Bingham and Fry <d-cite key="bingham-fry"></d-cite>
	* Fry and Burke <d-cite key="fry-burke"></d-cite>



[<img align="top" src="/assets/pdf/teaching/2024-Statistical-Models/bingham_fry.png" alt="drawing" width="48%"/>](https://link.springer.com/book/10.1007/978-1-84882-969-5)
[<img align="top" src="/assets/pdf/teaching/2024-Statistical-Models/fry_burke.png" alt="drawing" width="49%"/>](https://www.mheducation.co.uk/quantitative-methods-in-finance-using-r-9780335251261-emea-group)



- **Secondary References**: In addition we recommend the following

   * **Probability & Statistics Manual**: Casella and Berger <d-cite key="casella-berger"></d-cite> 
   * **Easier Probability & Statistics Manual**: DeGroot and Schervish <d-cite key="degroot"></d-cite>
   * **Concise Statistics with R**: Dalgaard <d-cite key="dalgaard"></d-cite>
   * **Comprehensive R manual**: Davies <d-cite key="davies"></d-cite>