## DAILY STUFF
- [ ] Read and annotate 1 paper
- [x] continue with obsidian vault structuring, add the new zotero integration template into this vault which is still using the old one
- [ ] Study a chapter
	AIC BIC
- [ ] https://youtube.com/playlist?list=PLDcUM9US4XdPz-KxHM4XHt7uUVGWWVSus&si=RloAIEYtwcKyUV4p
	- 1 chapter 
- [ ] change attachments structure
- [x] https://forum.obsidian.md/t/zotero-integration-import-templates/36310/101 
## **040625**
**questions**:
- seminars

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
![[Tracker 2025-05-22 20.20.06.excalidraw]]
 -   [ ] separating only for mother_highest_education (test_mother_highest_education vs father_highest_education)
	![[Tracker 2025-05-26 18.03.59.excalidraw]]
-  [ ] seperating only for father_highest_education (test_father_highest_education vs mother_highest_education
	![[Tracker 2025-05-26 18.10.10.excalidraw]]
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
      ![[Tracker 2025-05-19 15.58.30.excalidraw]]
- [x] Is it right?? to d oa manual reduction of dimensions and arbitrarily redefine the categories you're analysing e.g. instead of treating siblings as a continuous variable, you treat it as (0, 1, 2, 3+ siblings) because you realise you don't have sufficient data
- [ ] should we condense the non vaccinated components of parent_covid_dosage into one class such as "unvaxxed"? Because there's very little data to work with and they don't seem to vary so much (new categories will be unvaxxed, partial and full similar to the children's).
      - would something that captures their despise? for the vaccine be better, i.e. those who don't want to can be (feel no need to and against it), whilst we group ineligible and undecided together
- [x] (revisit 1) income, with mothers stay home and employment.
	- 0 employment status, unemployed, includes the following:  Students who are not working, Retirement (not working after retirement or early retirement), Stay-at-home mom, Unemployed
	- 0 mother stay home = mother not staying home
	- Thus 0, 0 (employment status and stay home) means mothers who aren't stay home moms in the traditional sense but are: uneployed, retired or students who aren't working (phd perhaps)
- [x] consult on the validity of ancova for the relationship between, [[age, age_group and siblings]] example (and if this should actually ever be used)
	- [x] continue to decide test_siblings vs sibligns
	- ![[Tracker 2025-05-14 14.31.06.excalidraw|600]]
- [ ]  test_child_siblings and birth order vs child_siblings and birth_order
![[Drawing 2025-05-14 13.34.12.excalidraw|700]]
 - Tried looking at siblings with respect to test_siblings but data isn't very helpful
 - ![[Tracker 2025-05-14 14.42.12.excalidraw]]
- [x] (Revisit 2) Combinations of mothers and fathers highest education
	- [x] do we have the grounds to remove employment status
![[Tracker 2025-05-16 13.05.38.excalidraw|700]]





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
![[Drawing 2025-05-13 17.48.15.excalidraw]]
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