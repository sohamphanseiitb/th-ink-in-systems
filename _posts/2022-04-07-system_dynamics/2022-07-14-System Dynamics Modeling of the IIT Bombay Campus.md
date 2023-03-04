---
layout: page
title: "System Dynamics Modeling - The Case of IIT Bombay campus"
author: "Soham Phanse"
categories: journal
tags: [documentation,sample]
---


Hey folks! To tie up everything we have seen so far, I will walk you through a simple and everyready case. It is about constructing a system dynamics model of the population of a particular university campus. Incidentally, as you might have guessed, this is one of the simplest population models since we hace strict rules with respect to increase in number of students, hence accurate estimates can be obtained and special statistical techniques are not required. The model with suitable (a lot :P) can be extended to construct models predicting a city or a nation wide population estimate.

Since you peeps should know the background, I was working to model the energy consumption trends on my university campus. Since energy consumption heavily depends on the numbers of users and usage per capita, my immediate task was to estimate the total populaiton living on campus. The framework starts with obtaining basic data about the number of students, the student to faculty ratio, administration staff, dependents living on campus and estimating admission rates for students, hiring and attrition rates for professors and other staff members on campus.

To give you an idea of how the student population on campus changes across the years, check this sketch below:

![Population Model](https://sohamphanseiitb.github.io/Think-in-Systems/assets/system-dynamics/population%20blog.jpg)

Obviously, the rate at which undergraduate students are admitted will be starkly different than graduate students.

Similarly, we can construct a model to estimate how the taching faculty grows over time. To simplify stuff, the Student to Faculty Ratio can be assumed to be constant, however it is better to assume it adaptable, since every uiversity strives to attain the best possible ration as mandated by national standards. The number distribution of undergraduate and graduate students on campus also affects the required amount of teaching staff. The Student to Faculty ratio in case of graduate students is expected to be higher than undergraduates. In that case, two different ratio estimates can be calculated, however it should be understood that there be a significant fraction of staff which will be teaching and advising at both levels. We can make assumptions about how the universities plans to implement policies to improve the ratio each year. The policies can be as follows:

- Case 1: If the ratio is higher than the mandate (low teaching staff strength)
  - Increase the hiring rate, vis a vis, hire more people every year. 
  - Reduce attrition rate, vis a vis, provide incentives to people to improve retention period
    -  Provide schemes like subsidized medical insurance, interest free loans, pension benefits and provident fund schemes

- Case 2: If the ratio is lower than the mandate (high teaching staff strength)
  -  Decrease the hiring rate, in extreme cases, new hiring can be frozen
  -  Improve performance vigilance, to keep under-performing staff in check and incentivise attrition

The administration staff on the other hand, is more trickier to model, since it doesn't have well defined ratios to be kept in check. A modest 3-5% growth can be assumed safely. If the university provides housing to teaching and other staff on campus and allows immediate family members to stay along, a rough number of 2 dependents per working members of staff can be assumed to calculate the total number of staff dependents. 

With these population sub-models of students, teaching and non-academic staff and dependents a fair estimate of the total population on the university campus can be obtained. This further can be combined with other models to estimate the per capita energy consumption in each category and ultimately total energy usage at domestic levels for personal use. 

For commercial uses, like computing and use in research equipment, outdoor lighting and common areas like gymnasiums, sports complexes, auditoriums the energy usage has to be calculated with data, since no modeling techniques can give accurate estimates. Constructing gymnasiums, new research labs on campus are discrete events by nature and cannot be predicted beforehand. In cases of infrastructural expansion, the total land area availability and the trend estimation timeline should also be considered.

All in all, if you see systems modeling can start with simple logic and building blocks which together can be assembled to produce useful results. Complex models can be built with simple models and layers of statistical estimates can be grafted onto propagative models to create models with can accurately estimate real world phenomena like business cycles, stock value predictions or the global world economic scenario. 
