## Updated causal model and considerations
![[50 Vaccine Uptake DAG-DAG 08-07-25.jpg]]
- diagram updated, colours:
	  - white, included but not an exposure of interest
	  - green a variable of interest that's been included
	  - grey, not included (and blue for birth order)
- remove birth order (when compared to the previous DAG), bc, if it is included and controlled for, it results in there being dependence as it's a collider -**but this depends on if we want to examine the direct or total effect??**
	- [causality - DAG: interpretation difference of TOTAL and DIRECT effect in terms of adjusting - Cross Validated](https://stats.stackexchange.com/questions/520426/dag-interpretation-difference-of-total-and-direct-effect-in-terms-of-adjusting)
- we can't include any of the parent's vaccination statuses other than perception because that'd result in us conditioning on colliders.

## Updated causal model and considerations
![[50 Vaccine Uptake DAG-DAG 08-07-25.jpg]]
- **This is the correctly adjusted DAG to examine overall effects**
- diagram updated, colours:
	  - white, included but not an exposure of interest (i.e. we are controlling for this)
	  - green a variable of interest that's been included
	  - grey, not included (and blue for birth order)
- remove birth order (when compared to the previous DAG), bc, if it is included and controlled for, it results in there being dependence as it's a collider -**but this depends on if we want to examine the direct or total effect??**
	- [causality - DAG: interpretation difference of TOTAL and DIRECT effect in terms of adjusting - Cross Validated](https://stats.stackexchange.com/questions/520426/dag-interpretation-difference-of-total-and-direct-effect-in-terms-of-adjusting)
- we can't include any of the parent's vaccination statuses other than perception because that'd result in us conditioning on colliders.

![[50 Vaccine Uptake DAG-DAG 140725_0]]


- **This is the correctly adjusted DAG to examine DIRECT effects**
- diagram updated, colours:
	  - white, included but not an exposure of interest (i.e. we are controlling for this)
	  - green a variable of interest that's been included
	  - grey, not included

## new causal Effects to focus on/include?
1. **Perception**: Choose a variable with regards to a child's parent's perception of vaccination/govt stuff
	- **reason**: though these factors aren't directly involved in predicting the child's vax uptake (from a family factors viewpoint), it is a strong predictor and thus explains some of the variance in the data. Including these factors will increase the accuracy of the model
	- **question**: is there a way to look at which variable i should include? ANOVA? PCA
	- **nominees**:
		- danger of infection
		- safety of sanctioned vaccines

	- ![[50 Vaccine Uptake DAG-heatmap for vaccination uptakes and parents perceptions|1558]]
2. Siblings over 18 shouldn't directly influence the uptake as they are presumably indep from their families. 
	- **questions**: but then, do you think older siblings can affect uptake as they're more educated and can advise their parents?
3. parents_time_since_covvax and dosage:
	- we will keep dosage bc time since covvax and dosage tell much of the same story and there isn't enough data for time since covvax?
## Investigating effect modification
![[50 Vaccine Uptake DAG 10-06-25.excalidraw]]
- previously I was looking at effect modifiers in terms of the causal relationships between the variables
- However, it should just be a case of me mapping out all possible interactions
- thus, i will remap everything and then draw up the necessary graphs and all shall be good: