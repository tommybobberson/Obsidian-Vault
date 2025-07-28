![[40 Attachments/50 Vaccine Uptake Tracker]]
## Stuff to work on 
## DAILY STUFF
- [ ] Read and annotate 1 paper
- [ ] Study a chapter
	AIC BIC
- [ ] https://youtube.com/playlist?list=PLDcUM9US4XdPz-KxHM4XHt7uUVGWWVSus&si=RloAIEYtwcKyUV4p
	- 1 chapter 
- [x] change attachments structure
	- [x] Consider using i,age paste renamer instead
	- [x] Consider seperating literature notes and the reference itself?
- [x] https://forum.obsidian.md/t/zotero-integration-import-templates/36310/101
- [ ] try diff note taking structures :
	- how to sort class notes, do you use 
	- [ ] one note then import into obsidian
	- [ ] put them directly in excalidraw
	- how to take notes 
	- [x] take notes along side the pdf, copy and pasting where needed or  ==actually not bad==
	- [ ] just annotating on the pdf 
	-  how to store class notes themselves
	- [ ] put them all in resources 
	- [ ] put them in fleeting notes and then link them to concepts or create these links while you are note taking
	

## 300725
- [ ] work on exploratory segmented model

	- [ ] check assumptions for logistic regression between (age, age_cat and uptake), or is it a linear regression, given we are estimating the **proportion** of individuals at every age group???
		- but the probability should translate to the proportion of individuals at every age group
	- [ ] can test interaction term model first too to see if it's sufficient
	- [ ] else figure out the difference between segmented lines and an interaction term
	- [ ] fit model and compare it with the data that we obtained during exploratory analysis
	- [ ] model diagnostics
- [ ] work on slides for wolbachia
- [ ] read up on [[10 Propensity Score]]

## 160725
**To-cover**:
- [x] Debt and mortgage
- [x] All of the effect mod stuff, [[50 Vaccine Uptake DAG]]
	- [x] How do i know if effect mod between child_siblings, age_cat and age_of_interest is 2 x 2 way or a 3 way interaction?
	- ![[50 Vaccine Uptake Tracker 16-07-25.excalidraw]]
## **100725
to cover**:
- what's our variable of interest? do we have 2, no vax and full vax? or do we have one outcome which is the odds of getting fully vaccinated
	- bc when you're running a regression model, you're loooking at all the data (vaccine status = 0, 1 and 2)

## **110625**
**ad-hoc task, the diagrams:**
- [ ] child_age, age_cat
- [ ] parents_highest_education, income

to-cover:
- The mystery of why the coefficient of vax uptake regarding parents who held a postgraduate qualification was lower than other qualifications, possibilities:
	![[50 Vaccine Uptake Tracker 04-06-25.excalidraw]]
- [x] revise dag once more and how to identify effect modifiers
	- we can probably remove the proxies which are the parent's vaccination uptakes given they don't confound anything or aren't related causally (but they are a good indicator so maybe not)
	- keep parents intentions/attitudes toward future vaccination?
	- test for parents' knowledge of vaccines/attitudes towards vaccines and how that impacts uptake
	- new interaction terms being investigated
	- remove parents_marital_status / child_parents
- [x] ask if we should keep the parental vaccination terms bc they have no causal effect on vaccine uptake. Or if you'd like to just examine the association between parental uptake / child's updatke Or if you want to view parental Vax as another potential outcome?
- [x] cover new variables and add them to the dag
	- perception as another outcome variable? and can we, from this, investigate the correlation between perception and actual uptkae
	- mortgage: 0 vs any, across levels
	- debt: 0 vs any, across levels
	- working hours weekly, father and mother
	- responding parent childcare hours daily
-  [ ] potential vaccine uptake figures??
	- age-category and school year

**Questions:**
- [ x] checl if can book conference room
- [ ] Read and annotate 1 paper
- [x] maybe pdf++?
- [ ] Study a chapter
	AIC BIC
- [ ] https://youtube.com/playlist?list=PLDcUM9US4XdPz-KxHM4XHt7uUVGWWVSus&si=RloAIEYtwcKyUV4p
	- 1 chapter 
- [x] change attachments structure
	- [x] Consider using i,age paste renamer instead
	- [x] Consider seperating literature notes and the reference itself?
- [x] https://forum.obsidian.md/t/zotero-integration-import-templates/36310/101
- [ ] try diff note taking structures :
	- how to sort class notes, do you use 
	- [ ] one note then import into obsidian
	- [ ] put them directly in excalidraw
	- how to take notes 
	- [x] take notes along side the pdf, copy and pasting where needed or  ==actually not bad==
	- [ ] just annotating on the pdf 
	-  how to store class notes themselves
	- [ ] put them all in resources 
	- [ ] put them in fleeting notes and then link them to concepts or create these links while you are note taking
	- [ ] 

## 160725
**To-cover**:
- [ ] Debt and mortgage
- [ ] All of the effect mod stuff
## **100725
to cover**:
- what's our variable of interest? do we have 2, no vax and full vax? or do we have one outcome which is the odds of getting fully vaccinated
	- bc when you're running a regression model, you're loooking at all the data (vaccine status = 0, 1 and 2)

## **110625**
**ad-hoc task, the diagrams:**
- [ ] child_age, age_cat
- [ ] parents_highest_education, income

to-cover:
- The mystery of why the coefficient of vax uptake regarding parents who held a postgraduate qualification was lower than other qualifications, possibilities:
	![[50 Vaccine Uptake Tracker 04-06-25.excalidraw]]
- [x] revise dag once more and how to identify effect modifiers
	- we can probably remove the proxies which are the parent's vaccination uptakes given they don't confound anything or aren't related causally (but they are a good indicator so maybe not)
	- keep parents intentions/attitudes toward future vaccination?
	- test for parents' knowledge of vaccines/attitudes towards vaccines and how that impacts uptake
	- new interaction terms being investigated
	- remove parents_marital_status / child_parents
- [x] ask if we should keep the parental vaccination terms bc they have no causal effect on vaccine uptake. Or if you'd like to just examine the association between parental uptake / child's updatke Or if you want to view parental Vax as another potential outcome?
- [x] cover new variables and add them to the dag
	- perception as another outcome variable? and can we, from this, investigate the correlation between perception and actual uptkae
	- mortgage: 0 vs any, across levels
	- debt: 0 vs any, across levels
	- working hours weekly, father and mother
	- responding parent childcare hours daily
-  [ ] potential vaccine uptake figures??
	- age-category and school year

**Questions:**
- [ ] when reading a paper, do you read from start to end? or do you go in looking for what you want

## **040625**
**learn**:
- [ ] different regression fitting methods
**to -do**:
- [ ] make new vaccine uptake categories for the complement of fully vaxxed and the complement of unvaxxed
- [x] when reading a paper, do you read from start to end? or do you go in looking for what you want

## **040625**
**learn**:
- [ ] different regression fitting methods
**to -do**:
- [ ] make new vaccine uptake categories for the complement of fully vaxxed and the complement of unvaxxed
- [x] add debt and mortgage
	
- [x] look at any other variables that you might include?, shortlisted: **and for those chosen, update the DAG to see if it's relevant**
	- Q12: job type (desk job, talking, using one's body)
	- ==Q13: working hours per week, spouse and respondent==
	- Q20: insurance
	- Q23: housing type
	- ==Q31.11 and Q31.10 : time spent on childcare== & time spent on housework
	- Q82: Vice behaviour?
- [ ] check the uptake of postgrads with income (what income level postgrads are located in, and what could have caused their interaction)
- [ ] make sure income is continuous for regression
- [ ] look at the interaction with income for ALLL levels of education, father and mother
- [ ] compare models for parents_highest-ed and treating mom and dad seperately
- [x] compress technical and JC
- [x] get rid of mother_stay_home

**questions**:
- [x] in the regressions we ran, what are the equations of interest?
- Either parent who was a postgrad gave a different gradient **with income** so it should be an interaction between income and each parent's education 
- another theory is that only the parents highest education affects the uptake
- **notable points**:
	- JC and VC for mothers result in roughly the same uptake
	- TC and VC result in vastly different uptakes
	- PG mothers and fathers both show an increased uptake of full coverage and a decreased uptake of no coverage at all when only education was included, but not when income was included
- [x] seminars
- [x] do we want to include all the new variables that we have been using as covariates in our dag as direct exposures too?
- [ ] do i focus on learning now?? or try to apply even if i don't know what it's doing

**to do**:
- remove vulnerable individuals from the DAG and everything else and ignore the effect too
- check if the confidence intervals are limited by the range of the axes themselves
- weight by sample size
- run regressions for EDA
- consdier removing siblings over 18
- 

## **280525**
**questions**:
- [x] whilst we are removing vulnerable individuals, given that it seems like it might have a significant interaction with test_household_income, is it possible to include a terms' interactions without including hte actual term itself? (vulnerable_indivs_income)
- [x] which dag to maintain 
	- and are the changes alright, removed the following:
	  - **household_total -> household_income** (because when we're looking at total household income, we only have to account for the number of parents, and siblings over 18 who are most likely working, idk is it common for children under 18 to be working; or if they do i don't think it contributes significantly
	  - **child_siblings -> age_of_interest** (because the number of siblings the child has won't affect when the COI was born)
	  - **birth order -> age_of_interest** (same reason as above)
	  - **parent_chronic_illness -> test_parents_marital_status** and replaced with **parent_chronic_illness <-parent_1_age -> test_parents_marital_status** (as age might affect divorce rates and chronic illness)
- [x] How to deal with cyclic graph
- [x] what do we do with outliers in the process of EDA

**To cover**:
- [x] How stratifying education by TC, VS and JC affects vax uptake as compared to lumping them together:
		- Current assumption: only highest educations out of both parents impacts the uptake of the vaccine. That means that, for a given 
	- [ ] seperating the technical college/junior college category into TC, VS and JC for both mothers' and fathers' highest education (test_mother_highest_education vs test_father_highest_eduction)
![[50 Vaccine Uptake Tracker 1]]
 -   [ ] separating only for mother_highest_education (test_mother_highest_education vs father_highest_education)
	![[50 Vaccine Uptake Tracker 2]]
-  [ ] seperating only for father_highest_education (test_father_highest_education vs mother_highest_education
	![[50 Vaccine Uptake Tracker 3]]
## **210525**
**Changes to update**:
- [ ]  Converted the number of vulnerable individuals to the presence of vulnerable individuals in a household due to the small sample of households with $>=1$ vulnerable individuals in the first place
- [ ] Convert the number of grandparents to the presence of grandparents
- [ ] ask about research and seminars etc.
- [ ] limit household total to 8 indivs
- [x] make another test_education 
	- if education = 4 -> vocational school
	- if education = 5 and male -> technical college
	- if educationi = 5 and female -> Junior college

**To-do**:
- [ ] is it possible to run some sort of weight on the samples to increase the samples for the richer ppl , refer to |vulnerable_indivs_income|
- [ ] learn to add bayesian intervals
- [x] change vulnerable individuals to the presence of vulnerable individuals
- [ ] Convert the number of grandparents to the presence of grandparents
- [x] Add children over 18 too
- [ ] list parents_highest_education vs mother_highest_education and father_highest_education as different models to do?
- [x] stratify between JC and TC for father_highest_education vs mother_highest_education
- [ ] try replacing birth order with children over 18 in plots especially for child_siblings_age_of_interest_birth_order
- [ ] Remove vulnerable individuals as a whole (as a predictor but maybe not an effect modifier)
questions:
- [x] Is it ok to look at individual level interactions before looking at interactions on a whole level? (look at example of household_total * child_grand and household_total_test_parents_marital_status first)
      ![[50 Vaccine Uptake Tracker 4]]
- [x] Is it right?? to d oa manual reduction of dimensions and arbitrarily redefine the categories you're analysing e.g. instead of treating siblings as a continuous variable, you treat it as (0, 1, 2, 3+ siblings) because you realise you don't have sufficient data
- [ ] should we condense the non vaccinated components of parent_covid_dosage into one class such as "unvaxxed"? Because there's very little data to work with and they don't seem to vary so much (new categories will be unvaxxed, partial and full similar to the children's).
      - would something that captures their despise? for the vaccine be better, i.e. those who don't want to can be (feel no need to and against it), whilst we group ineligible and undecided together
- [x] (revisit 1) income, with mothers stay home and employment.
	- 0 employment status, unemployed, includes the following:  Students who are not working, Retirement (not working after retirement or early retirement), Stay-at-home mom, Unemployed
	- 0 mother stay home = mother not staying home
	- Thus 0, 0 (employment status and stay home) means mothers who aren't stay home moms in the traditional sense but are: uneployed, retired or students who aren't working (phd perhaps)
- [x] consult on the validity of ancova for the relationship between, [[age, age_group and siblings]] example (and if this should actually ever be used)
	- [x] continue to decide test_siblings vs sibligns
	- ![[50 Vaccine Uptake Tracker 5|600]]
- [ ]  test_child_siblings and birth order vs child_siblings and birth_order
![[50 Vaccine Uptake Tracker 6|700]]
 - Tried looking at siblings with respect to test_siblings but data isn't very helpful
 - ![[50 Vaccine Uptake Tracker 7]]
- [x] (Revisit 2) Combinations of mothers and fathers highest education
	- [x] do we have the grounds to remove employment status
![[50 Vaccine Uptake Tracker 8|700]]





## **140525
**Follow up**:
- [ ] differentiate between junior and technical college
- [x] look at income and uptake for each cobmination of mothers and fathers highest education
- [x] double check exact defnition for 0 0 for income_mother_stay_home_employment
- [x] Consdier removing employment status after that

questions :
- [ ] grouped regression only categorical 
- [ ] Is simpson's paradox the same as confounding and can it only occur with confounding
- Does an absence of points (in the lower income values) indicate anything? Or does it just reflect the fact that income affects the uptake of the vaccine. But the levels of education that extend to each level of income also differ. That means that ther is some sort of interaction between education, income and thus uptake 
	e.g. for post grad:
	    edu -> income -> uptake
	    postgrad -> income > category 2 -> uptake is naturally higher.
- [ ] get opinion on if it's a better idea to stratify age groups by 0.5 years or 1 year, use the example of the age_child_siblings_ plots and also then
- [ ] continuing from the 0.5 years dilemma, how to categorise them by age group too, and based on school year thing? [School Grade and Age Structures in Japan - PLAZA HOMES](https://www.realestate-tokyo.com/living-in-tokyo/education/school-grades-ages/)
- [ ] Schooling level, age and uptake causality, age_cat is a mediator here..
![[50 Vaccine Uptake Tracker 9]]
**To cover**:
- [x] 
### **300425**
**progress**:
- stopped at list of plots [23]

**to fix:**
- [x] fix the birth order thing, and child siblings thing to include children over 18
- [x] see how the effect of siblings affects the uptake (based on siblings all < 18 and siblings < 18 + >18) -> and use this to consider if you want to remove household total
- [x] just keep plotting and try to look for cases of effect modification, then we can just ignore effect modification


**to cover**:
- [x] check definition of child_siblings (only under 18?) and birth_order (total)
- [x] propensity score
- [x] do we want to bunch all our variables of interest (i.e. familial factors) into one variable or do we want to keep them seperate - **no pca, keeo seperate**

**to do**
- see if the effects roughly add up(in terms of association), because if they're independent their effect should add up sorta
- look for textbook that talks about the interaction
- its ok to include both categorical and numerical vars
- check the significance between vulnerable indivduals and gradparents (R^2 = 0.12) because when there are less discrete values, the significance changes even though R^2 is small; also for child_parents and test_household_income
- [x] ask about propensity score
- [ ] see how household size changes with other subgroups, plot stuff that's related together (for continuous vars, chud siblings, parents, grand etc.) -- see if it's redundant
- [ ] plot employment status, marital status, household income tgth (and combinations of parents employment statuses)
- [ ] plot childs' uptake for each parent covid dose and parents_time_since_covvax
- [ ] remove parents_time_since
- [ ] would parents influenza uptake affect children's uptake of influenza? (generate the model with and without parents influenza uptake? it's a confounder)
- [ ] adjust birth order by age and household composition (sibling number too)
- [x] remove marital status
- [x] remove sisters and brothers
- [ ] treat income as a linear continuous numerical variable (use the midpoint of the bin)
- [x] combine junior high and high school
- [x] start classing chronic illnesses together --> bunch everything together, basically use chronic illnesses
- (auto immune diseases)
	- allergic rhinitis
	- asthma
	- dermatitis
- respiratory related
	- COPD
	- pneumonia
	- asthma
- Dental
	- caries
	- periodontitis
- Mental
	- Depression
	- Psychiatri other
- cancer
- stroke
- diabetes
- kidney disease
- dyslipidemia
- immune abnormalities
- [x] include stratified chronic illness graph in suppleementary materials
### **280425**
**to do**
- [x] filtered invalid results -- what else should I filter upon
- [x] added confidence intervals for
	- chronic illnesses
	- education levels
- [ ] plotted pairs plots to identify things that are linearly correlated
- [ ] plot things that indeed do have a linear relationship
	- [ ] check for residuals? (between themselves, to confirm that they do indeed have a linear r/s
	- [ ] check for collinearity in categorical and numerical variables

**to cover**
-  consult all blue cells on things to remove - reference plots
- plots 
	- [x] parents industry of work (non test)
	- [x] mother and father employment status (non test)
	- [x] parents influenza vaccination status (non test)
	- [x] parents time since cov vaccination (non test)
	- [x] birth order (non test)
	- [x] marital status (test)
	- [x] unstratified incomes vs stratified (test)
	- [x] newly stratified education (test)
	- [x] chronic illnesses (test) with confindence intervals

- questions
	- [x] we plot to determine non-linear r/ss between the continuous and numerical variables but what about logistic regression, technically it doesn't matter? 
	- [ ] what do i do with these intercorrelated relationships? e.g. mother employment, father employment and mother stay home - **ans, you determine how they interact within the model e.g. X1 + X2 or X1xX2
	- [x] What if there's a mix of continuous and categorical variables - what typa model do we use? Or is it wiser to convert the numerical variables into categories
	- [x] When doing EDA/calculating correlation matrices etc, should I only take the subset where there is a child of interest? (so that there's no effect modification, 
	- [ ] 
- suggestions
	- [ ] Remove sisters and brothers?