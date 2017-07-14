# Titanic Analysis using Tableau

## Summary
The goal of this project is to highlight the reasons which may have led people to either survive or die in the Titanic disaster.
Out of the various features available like Pclass, Embarked, Family members on board, Sex, Ages, etc we will look some particular ones that will lead us to concluding that the feature affected the survival of the people.

> 
[Link](https://public.tableau.com/profile/vikram3033#!/vizhome/TitanicVIZ-DAND/TitanicDataAnalysis) to the project on Tableau public

## Design decisions
Various decisions to model a plot, marks a certain way
Decisions taken after the feedback

## Feedback
I received feedback about my viz from 2 people. Below were some of points they mentioned and I incorporated the changes accordingly

**Feedback 1** => I am recording below the exact concerns pointed out by reader 1:
```
I feel below questions should be modified for better grasp of the chart that follows:

Q1. A family always supports you, even on Titanic
Q2. Did people from certain class belong to certain place

Q3. Also, chart explaining 'how many people had how many dependents' is a bit misleading when you hover anywhere inside a circle as it shows 'Dependents 0 Family members 161'.

Hope this helps :)
```

Below are the modifications:

Q1. A family always supports you, even on Titanic:
This has now been changed to:
**Does having a family member actually increase your chances of survival?**

Q2. Did people from certain class belong to certain place
This has been modified to:
**Was the Pclass of the people in any way related to places people boarded the Titanic from?**

Q3. Also, chart explaining 'how many people had how many dependents' is a bit misleading when you hover anywhere inside a circle as it shows 'Dependents 0 Family members 161'.
This was by far a very important the reader pointed out. When I cross checked, I almost changed 2 of my visualizations and also modified a calculated field. Also, I changed the count variable to _total records_ which made more sense rather that sum(Family Members).

__Prior to feedback__:
I renamed the _Sib Sp_ field to _Dependents_. I plotted 2 charts which showed whether having a dependent on board increases chances of survival.

__After the feedback__:
What I actually wanted to point out was that, whether having a family member (parents, children, spouse, siblings) affect the survival. I created another field and named it _Family Members_ which is a sum of _Sib Sp_ and _Parch_. Also, I had created field called _is Dependents_ which has true or false depending on whether a person has a dependent. Now the new field I created is named _Has Family Members_ which sounds correct rather than _is Family Members_. This feedback point actually helped me change my plots which were not that meaningful.

## Resources
All the links to the references if online and names if offline
