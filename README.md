
# Northwind Traders Business Exploration

## Northwind Database

The Northwind database is a sample database used by Microsoft to demonstrate the features of some of its products, including SQL Server and Microsoft Access. The database contains the sales data for Northwind Traders, a fictitious specialty foods export import company.

<img src='https://raw.githubusercontent.com/learn-co-curriculum/dsc-mod-3-project/master/Northwind_ERD_updated.png'>

## Goal
In this statistical analysis, we perform hypothesis tests to answer the following questions for Northwind Traders:  
#### Question 1
**_Does discount amount have a statistically significant effect on the quantity of a product in an order? If so, at what level(s) of discount?  
#### Question 2
**_Is there a statistically significant difference in the level(s) of discount offered by UK employees and USA employees?_**
**_Does the level(s) of discount offered by US employees have a statistically significant effect on the quantity ordered? If so, at what level(s) of discount?_**
**_Does the level(s) of discount offered by UK employees have a statistically significant effect on the quantity ordered? If so, at what level(s) of discount?_**
#### Question 3
**_Does the age of the employee have a statistically significant effect on number of orders processed?_**
**_Does having manager in your title have a statistically significant effect on number of orders processed?_**
**_Does the age of the employee have a statistically significant effect on the quantity of a product in an order?_**
**_Does having manager in your title have a statistically significant effect on quantity ordered?_**
#### Question 4
**_For each category type of product, does the season in which the order was placed have a statistically significant effect on the quantity of a product in an order?_**
#### Question 5
**_Does shipping company used have a statistically significant effect on the freight cost of shipping?_**
#### Question 6
**_Does category of product have a statistically signficiant effect on processing time? If so, which ones?_**
**_Does having a discount on the order have a statistically significant effect on processing time?_**
**_Does size of order have a statistically signficant effect on processing time?_**
**_Does shipping company have a statistically significant effect on processing time?_**

## Methodology

For answering our questions, we conducted one-tailed ANOVA tests followed by Tukey HSD Post-HOC tests afterwards to find the where the difference in mean is observed if there is one.

### Question 1
#### Does discount amount have a statistically significant effect on the quantity of a product in an order? If so, at what level(s) of discount?

$H_0$: there is no significant difference in quantity ordered due to discount  
$H_\alpha$: there is a significant difference in order quantity due to discount

#### At what level(s) of discount is there a statistically significant difference in quantity ordered?

$H_0$ (for each level): there is no significant difference in quantity ordered due to that specific discount level  
$H_\alpha$ (for each level): there is a significant difference in order quantity due to that specific discount level

### Question 2
#### Is there a statistically significant difference in the level(s) of discount offered by UK employees and USA employees?

$H_0$: there is no significant difference in level(s) of discount offered by the two countries  
$H_\alpha$: there is a significant difference in level(s) of discount offered by the two countries

#### Does the level(s) of discount offered by US employees have a statistically significant effect on the quantity ordered? If so, at what level(s) of discount?

$H_0$ (for each level): there is no significant difference in quantity ordered due to that specific discount level  
$H_\alpha$ (for each level): there is a significant difference in order quantity due to that specific discount level

#### Does the level(s) of discount offered by UK employees have a statistically significant effect on the quantity ordered? If so, at what level(s) of discount?

$H_0$ (for each level): there is no significant difference in quantity ordered due to that specific discount level  
$H_\alpha$ (for each level): there is a significant difference in order quantity due to that specific discount level

### Question 3
#### Does the age of the employee have a statistically significant effect on number of orders processed?

$H_0$: there is no significant difference in total sum of orders processed due employee age  
$H_\alpha$: there is a significant difference in total sum of orders processed due to employee age

#### Does having manager in your title have a statistically significant effect on number of orders processed?

$H_0$: there is no significant difference in total sum of orders processed due to the employee making order having a managerial position  
$H_\alpha$: there is a significant difference in total sum of orders processed due to the employee making order having a managerial position

#### Does the age of the employee have a statistically significant effect on the quantity of a product in an order?

$H_0$: there is no significant difference in quantity ordered due employee age  
$H_\alpha$: there is a significant difference in order quantity ordered due to employee age

#### Does having manager in your title have a statistically significant effect on quantity ordered?

$H_0$: there is no significant difference in quantity ordered due to the employee making order having a managerial position  
$H_\alpha$: there is a significant difference in order quantity ordered due to the employee making order having a managerial position

### Question 4
#### For each category type of product, does the season in which the order was placed have a statistically significant effect on the quantity of a product in an order?

$H_0$: there is no significant difference in quantity ordered due to season in which order was placed  
$H_\alpha$: there is a significant difference in order quantity ordered due to season in which order was placed

### Question 5
#### Does shipping company used have a statistically significant effect on the freight cost of shipping?

$H_0$: there is no significant difference in freight cost due to shipper  
$H_\alpha$: there is a significant difference in freight cost due to shipper

### Question 6
#### Does category of product have a statistically signficiant effect on processing time? If so, which ones?

$H_0$: there is no significant difference in processing time due to category of product  
$H_\alpha$: there is a significant difference in order quantity due to category of product

#### Does having a discount on the order have a statistically significant effect on processing time?

$H_0$: there is no significant difference in processing due to discount being applied  
$H_\alpha$: there is a significant difference in processing due to discount being applied

#### Does size of order have a statistically signficant effect on processing time?

$H_0$: there is no significant difference in processing time due to quantity ordered  
$H_\alpha$: there is a significant difference in processing time due to quantity ordered

#### Does shipping company have a statistically significant effect on processing time?

$H_0$: there is no significant difference in processing time due to shipper  
$H_\alpha$: there is a significant difference in processing time due to shipper

## Understanding Database

For this hypothesis, be sure to specify both the **_null hypothesis_** and the **_alternative hypothesis_** for your question.  You should also specify if this is one-tail or a two-tail test.

For online students, there will be four deliverables for this project:

1. A **_Jupyter Notebook_** containing any code you've written for this project. This work will need to be pushed to your GitHub repository in order to submit your project.
2. An organized **README.md** file in the GitHub repository that describes the contents of the repository. This file should be the source of information for navigating through the repository.
3. A **_[Blog Post](https://github.com/learn-co-curriculum/dsc-welcome-blogging)_**.
4. An **_"Executive Summary" PowerPoint Presentation_** that explains the hypothesis tests you ran, your findings, and their relevance to company stakeholders.  

Note: On-campus students may have different delivarables, please speak with your instructor. 

### Jupyter Notebook Must-Haves

For this project, your Jupyter Notebook should meet the following specifications:

**_Organization/Code Cleanliness_**

* The notebook should be well organized, easy to follow, and code is commented where appropriate.  
<br>  
    * Level Up: The notebook contains well-formatted, professional looking markdown cells explaining any substantial code. All functions have docstrings that act as professional-quality documentation.  
<br>      
* The notebook is written to technical audiences with a way to both understand your approach and reproduce your results. The target audience for this deliverable is other data scientists looking to validate your findings.  
<br>    
* Any SQL code written to source data should also be included.  

**_Findings_**

* Your notebook should clearly show how you arrived at your results for each hypothesis test, including how you calculated your p-values.   
<br>
* You should also include any other statistics that you find relevant to your analysis, such as effect size.

### Blog Post Must-Haves

Refer back to the [Blogging Guidelines](https://github.com/learn-co-curriculum/dsc-welcome-blogging) for the technical requirements and blog ideas.


### Executive Summary Must-Haves

Your presentation should:

* Contain between 5-10 professional quality slides detailing:
<br>  
    * A high-level overview of your methodology  
    <br>  
    * The results of your hypothesis tests  
    <br>  
    * Any real-world recommendations you would like to make based on your findings (ask yourself--why should the executive team care about what you found? How can your findings help the company?)  
    <br>  
* Take no more than 5 minutes to present  
<br>  
* Avoid technical jargon and explain results in a clear, actionable way for non-technical audiences.
