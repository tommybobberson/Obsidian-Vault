---
category: literaturenote
aliases:
tags: propensity score matching, read
citekey: austin_2011
doi: 10.1080/00273171.2011.568786
status: unread
dateread: 
---
# [An Introduction to Propensity Score Methods for Reducing the Effects of Confounding in Observational Studies](zotero://select/library/items/KM8JD6NP)
> [!Cite]
> 1  Austin PC. An Introduction to Propensity Score Methods for Reducing the Effects of Confounding in Observational Studies. _Multivariate Behavioral Research_ 2011;**46**:399–424. [https://doi.org/10.1080/00273171.2011.568786](https://doi.org/10.1080/00273171.2011.568786).

>[!Synth]  
>**Contribution**::  
>  
>**Related**:: 
>
>


>[!md]
> **FirstAuthor**:: Austin, Peter C.  
~    
> **Title**:: An Introduction to Propensity Score Methods for Reducing the Effects of Confounding in Observational Studies  
> **Year**:: 2011   
> **Citekey**:: austin_2011  
> **itemType**:: journalArticle  
> **Journal**:: *Multivariate Behavioral Research*  
> **Volume**:: 46  
> **Issue**:: 3   
> **Pages**:: 399-424  
> **DOI**:: 10.1080/00273171.2011.568786    

> [!LINK] 
>
>  [Full Text PDF](file://C:\Users\kevin\Zotero\storage\DZ9UXJJD\Austin%20-%202011%20-%20An%20Introduction%20to%20Propensity%20Score%20Methods%20for%20Reducing%20the%20Effects%20of%20Confounding%20in%20Observational.pdf).

> [!Abstract]
>
> The propensity score is the probability of treatment assignment conditional on observed baseline characteristics. The propensity score allows one to design and analyze an observational (nonrandomized) study so that it mimics some of the particular characteristics of a randomized controlled trial. In particular, the propensity score is a balancing score: conditional on the propensity score, the distribution of observed baseline covariates will be similar between treated and untreated subjects. I describe 4 different propensity score methods: matching on the propensity score, stratification on the propensity score, inverse probability of treatment weighting using the propensity score, and covariate adjustment using the propensity score. I describe balance diagnostics for examining whether the propensity score model has been adequately specified. Furthermore, I discuss differences between regression-based methods and propensity score-based methods for the analysis of observational data. I describe different causal average treatment effects and their relationship with propensity score analyses.
>.
> 

--- 
%% begin notes %%
## Main ideas:
- 
## Methodology:
- 
## Results:
- 
## Key points:
- 
%% end notes %%
## Reading notes
%% begin annotations %%


*Imported: 2025-07-19 15:07*

### ⭕ Very important or questionable

> [!quote|red]+ Highlight ([page. 7](zotero://open-pdf/library/items/DZ9UXJJD?page=7&annotation=WQKMEYPD))
> Schafer and Kang (2008) suggest that, within the matched sample, the treated and untreated subjects should be regarded as independent. In contrast to this, Imbens (2004) suggests that, when using a matched estimator, the variance should be calculated using a method appropri- ate for paired experiments. I argue that the propensity score matched sample does not consist of independent observations. Rather, treated and untreated subjects within the same matched set have similar values of the propensity score. Therefore, their observed baseline covariates come from the same mul- tivariate distribution 

> [!quote|red]+ Highlight ([page. 9](zotero://open-pdf/library/items/DZ9UXJJD?page=9&annotation=TD3FPBZ7))
> there are theoretical arguments for matching on the logit of the propensity score, as this quantity is more likely to be normally distributed, and for using a caliper width that is a proportion of the standard deviation of the logit of the propensity score. 
> - **Follow up**

> [!quote|red]+ Highlight ([page. 11](zotero://open-pdf/library/items/DZ9UXJJD?page=11&annotation=5Z6664YX))
> uses weights based on the propensity score to create a synthetic sample in which the distribution of measured baseline covariates is independent of treatmentassignmen 
> - **does that mean that, propensity score is definitive and there is no need to ensure a comparative distribution of covariates?**

> [!quote|red]+ Highlight ([page. 15](zotero://open-pdf/library/items/DZ9UXJJD?page=15&annotation=PMPMN998))
> it is not influenced by sample size and allows for the comparison of the relative balance of variables measured in different units 
> - **What does different units here mean?**

> [!quote|red]+ Highlight ([page. 18](zotero://open-pdf/library/items/DZ9UXJJD?page=18&annotation=623K5C6P))
> in many settings,most subject-level baseline covariates likely affect both treatment assignment and the outcome. Therefore, in many settings, it is likely that one can safely include all measured baseline characteristics in the propensity score model. 
> - **Be cautious snd plot out the causal structures**

> [!quote|red]+ Highlight ([page. 21](zotero://open-pdf/library/items/DZ9UXJJD?page=21&annotation=C3SZNIAP))
> in some settings, insufficient outcomes may be observed to allow oneto adequately adjust for all baseline variables that one would like to include inthe regression model. 
> - **Small samples favour psm?**

### ⭐ Important or interesting

> [!quote|orange]+ Highlight ([page. 399](zotero://open-pdf/library/items/DZ9UXJJD?page=399&annotation=IPHUECVW))
> In particular, the propensity score is a balancing score: conditional on the propensity score, the distribution of observed baseline covariates will be similar between treated and untreated subjects. 
> - **revisit after you finish the paper**

> [!quote|orange]+ Highlight ([page. 4](zotero://open-pdf/library/items/DZ9UXJJD?page=4&annotation=PMK4NEIB))
> In an RCTthese two measures of treatment effects coincide because, due to randomization, the treated population will not, on average, differ systematically from the overall population 

> [!quote|orange]+ Highlight ([page. 8](zotero://open-pdf/library/items/DZ9UXJJD?page=8&annotation=NR4ZYVW5))
> When matching with replacement is used, variance estimation must account for the fact that the same untreated subject may be in multiple matched sets (Hill & Reiter, 2006). 

> [!quote|orange]+ Highlight ([page. 9](zotero://open-pdf/library/items/DZ9UXJJD?page=9&annotation=F3Z4ZRSA))
> optimal matching and found that optimal matching did no better than greedymatching in producing balanced matched samples. 

> [!quote|orange]+ Highlight ([page. 9](zotero://open-pdf/library/items/DZ9UXJJD?page=9&annotation=BL4DGGQK))
> no uniformly agreed upon definition ofwhat constitutes a maximal acceptable distance 

> [!quote|orange]+ Highlight ([page. 11](zotero://open-pdf/library/items/DZ9UXJJD?page=11&annotation=KVBNBG4K))
> weight is equal to the inverse of the probability of receiving the treatment that the subject actually received 
> - **the weight, through including the terms Z_i and (1 - Z_i) account for the likelihood of receiving or not receiving the treatment**

> [!quote|orange]+ Highlight ([page. 11](zotero://open-pdf/library/items/DZ9UXJJD?page=11&annotation=34RJB2L4))
> standardization 

> [!quote|orange]+ Highlight ([page. 15](zotero://open-pdf/library/items/DZ9UXJJD?page=15&annotation=EHU4FCE2))
> pooled standard deviation 
> - **Why pooled?**

> [!quote|orange]+ Highlight ([page. 16](zotero://open-pdf/library/items/DZ9UXJJD?page=16&annotation=SFY7CKPW))
> a set of criteria based on comparing the distribution of the propensity score between treated and untreated subjects 

> [!quote|orange]+ Highlight ([page. 16](zotero://open-pdf/library/items/DZ9UXJJD?page=16&annotation=UI2HAVDB))
> comparison of baseline covariates may be complemented by comparing the distribution of the estimated propensity score between treated and untreatedsubjects in the matched sample 
> - **You want a similar distribution and mean**

> [!quote|orange]+ Highlight ([page. 17](zotero://open-pdf/library/items/DZ9UXJJD?page=17&annotation=BFAHN4FD))
> criticized 

> [!quote|orange]+ Highlight ([page. 17](zotero://open-pdf/library/items/DZ9UXJJD?page=17&annotation=6Z4K6IMW))
> Recent research has indicated that this statistic provides no information as to whether the propensity score model has been correctly specified 
> - **Cstatistic doesnt tell you if the logistic regression or model used to generate the propensity score was wrong**

> [!quote|orange]+ Highlight ([page. 18](zotero://open-pdf/library/items/DZ9UXJJD?page=18&annotation=4A3YHGTD))
> using these two propensity score models did not result in theintroduction of additional bias but resulted in estimates of treatment effect with greater precision. 
> - **More matched pairs and lower MSE**

> [!quote|orange]+ Highlight ([page. 18](zotero://open-pdf/library/items/DZ9UXJJD?page=18&annotation=6LR9ZBL8))
> one should stress that the propen-sity score model should only include variables that are measured at baselineand not post-baseline covariates that may be influenced or modified by the treatment. 

> [!quote|orange]+ Highlight ([page. 19](zotero://open-pdf/library/items/DZ9UXJJD?page=19&annotation=PHCHMKWD))
> measure of treatment effect is said to be collapsible if the conditional andmarginal effects coincide. 

> [!quote|orange]+ Highlight ([page. 20](zotero://open-pdf/library/items/DZ9UXJJD?page=20&annotation=736DMEPC))
> aforementioned suggest that researchers need to carefully distinguish between marginal and conditional treatment effects. 

> [!quote|orange]+ Highlight ([page. 20](zotero://open-pdf/library/items/DZ9UXJJD?page=20&annotation=X58EDZGE))
> if theobjective of an observational study is to answer the same question as an RCT,the marginal effect may be of greater interest to researchers using observational da 
> - **Rcts and psms allow for the estimation of the effect on the whole population**

> [!quote|orange]+ Highlight ([page. 21](zotero://open-pdf/library/items/DZ9UXJJD?page=21&annotation=SIB4X2PL))
> there may be increased flexibility when outcomes (when binary or time-to-event in nature) are rare and treatment is common 
> - **Better for rare outcomes**

> [!quote|orange]+ Highlight ([page. 21](zotero://open-pdf/library/items/DZ9UXJJD?page=21&annotation=J8BWDPNH))
> If there are substantial differences in baseline covariates between treated and untreated subjects, this will be evident by either the small number of matched subjects 

> [!quote|orange]+ Highlight ([page. 21](zotero://open-pdf/library/items/DZ9UXJJD?page=21&annotation=TRMAACA7))
> observation that most strata consist primarily of either treated subjects or primarily of untreated subjects 
> - **Certain stratum are more likely to be treated than others**

> [!quote|orange]+ Highlight ([page. 22](zotero://open-pdf/library/items/DZ9UXJJD?page=22&annotation=Q756944E))
> Thus, just as randomization will, on average, result in bothmeasured and unmeasured covariates being balanced between treatment groups, so conditioning on the propensity score will, on average, result in measured baseline covariates being balanced between treatment groups 
> - **Only applies to measured covariates**

### ✅ Major statements

> [!quote|green]+ Highlight ([page. 10](zotero://open-pdf/library/items/DZ9UXJJD?page=10&annotation=H3ABCSP4))
> Stratification on the Propensity Score 
> - **A new thing, this is another method to use propensity scores, not matching**

> [!quote|green]+ Highlight ([page. 11](zotero://open-pdf/library/items/DZ9UXJJD?page=11&annotation=UPSYMPQP))
> Inverse Probability of Treatment Weighting Using the Propensity Score 
> - **not, PSM**

> [!quote|green]+ Highlight ([page. 12](zotero://open-pdf/library/items/DZ9UXJJD?page=12&annotation=3PJBATN6))
> Covariate Adjustment Using the Propensity Score 
> - **not psm**

### 📚 Ordinary notes

> [!quote|yellow]+ Highlight ([page. 400](zotero://open-pdf/library/items/DZ9UXJJD?page=400&annotation=YFWTI423))
> treatment selection is often influenced by subject characteristics 

> [!quote|yellow]+ Highlight ([page. 400](zotero://open-pdf/library/items/DZ9UXJJD?page=400&annotation=3A5CTEE4))
> one must account for systematic differences in baseline characteristics between treated and untreated subjects when estimating the effect of treatment on outcomes 

> [!quote|yellow]+ Highlight ([page. 4](zotero://open-pdf/library/items/DZ9UXJJD?page=4&annotation=Y5DAS44E))
> potential outcomes: Yi.0/ and Yi.1/ 
> - **Y for treated and untreated**

> [!quote|yellow]+ Highlight ([page. 4](zotero://open-pdf/library/items/DZ9UXJJD?page=4&annotation=CPDPAB3D))
> Yi.Yi D ZiYi.1/ C .1   Zi/Yi.0// 
> - **When z = 0, yi(1) and when z = 1 yi(0)**

> [!quote|yellow]+ Highlight ([page. 4](zotero://open-pdf/library/items/DZ9UXJJD?page=4&annotation=BLQQ32K8))
> ATE is the average effect, at the population level, of moving an entire population from untreated to treated 

> [!quote|yellow]+ Highlight ([page. 4](zotero://open-pdf/library/items/DZ9UXJJD?page=4&annotation=HSEZTE6N))
> is the average effect oftreatment on those subjects who ultimately received the treatment 
> - **As compared to the theoretical outcome where the treated individuals never received treatment**

> [!quote|yellow]+ Highlight ([page. 5](zotero://open-pdf/library/items/DZ9UXJJD?page=5&annotation=KZRA6BYJ))
> unbiased estimate of the ATE is EŒYi.1/ Yi.0/ D EŒY .1/ EŒY .0/ 

> [!quote|yellow]+ Highlight ([page. 5](zotero://open-pdf/library/items/DZ9UXJJD?page=5&annotation=II3TTEKS))
> I have that EŒY .1/jZ D 1 ¤ EŒY .1/ 

> [!quote|yellow]+ Highlight ([page. 5](zotero://open-pdf/library/items/DZ9UXJJD?page=5&annotation=5V93WRSZ))
> set of subjects all of whomhave the same propensity score, the distribution of observed baseline covariates will be the same between the treated and untreated subjects. 

> [!quote|yellow]+ Highlight ([page. 6](zotero://open-pdf/library/items/DZ9UXJJD?page=6&annotation=KQ8NEHF5))
> In observational studies, the true propensityscore is not, in general, known. However, it can be estimated using the study data 

> [!quote|yellow]+ Highlight ([page. 7](zotero://open-pdf/library/items/DZ9UXJJD?page=7&annotation=RM6W5YXH))
> Propensity score matching entails forming matched sets of treated and untreated subjects who share a similar value of the propensity score 

> [!quote|yellow]+ Highlight ([page. 7](zotero://open-pdf/library/items/DZ9UXJJD?page=7&annotation=8F4YYD4N))
> Once a matched sample has been formed, the treatment effect can be esti- mated by directly comparing outcomes between treated and untreated subjects in the matched sample. 

> [!quote|yellow]+ Highlight ([page. 7](zotero://open-pdf/library/items/DZ9UXJJD?page=7&annotation=RHTLRHQZ))
> outcome is continuous (e.g., a depression scale), the effect of treatment can be estimated as the difference between the mean outcome 

> [!quote|yellow]+ Highlight ([page. 7](zotero://open-pdf/library/items/DZ9UXJJD?page=7&annotation=XMYKPASV))
> dichotomous (self-report of the presence or absence of depression), the effect of treatment can be estimated as the difference between the proportion of subjects experiencing the event in each of the two groups (treated vs. untreated) 

> [!quote|yellow]+ Highlight ([page. 7](zotero://open-pdf/library/items/DZ9UXJJD?page=7&annotation=8BUDYPDU))
> Once the effect of treatment has been estimated in the propensity score matched sample, the variance of the estimated treatment effect and its statistical significance can be estimated 

> [!quote|yellow]+ Highlight ([page. 8](zotero://open-pdf/library/items/DZ9UXJJD?page=8&annotation=KJIJLEY4))
> In the context of an RCT, oneexpects that, on average, the distribution of covariates will be similar between treatment groups. 

> [!quote|yellow]+ Highlight ([page. 8](zotero://open-pdf/library/items/DZ9UXJJD?page=8&annotation=QP7A7PZT))
> untreated subject is included in at most one matched se 

> [!quote|yellow]+ Highlight ([page. 8](zotero://open-pdf/library/items/DZ9UXJJD?page=8&annotation=22PNR4FC))
> called greedy because at eachstep in the process, the nearest untreated subject is selected for matching to thegiven treated subject, even if that untreated subject would better serve as a match for a subsequent treated subject 
> - **Ie treated subjects are mqtched in order, not based on maximising the match**

> [!quote|yellow]+ Highlight ([page. 8](zotero://open-pdf/library/items/DZ9UXJJD?page=8&annotation=LXE7MH4Q))
> optimalmatching, in which matches are formed so as to minimize the total within-pair difference of the propensity score. 

> [!quote|yellow]+ Highlight ([page. 9](zotero://open-pdf/library/items/DZ9UXJJD?page=9&annotation=G8VLUIK8))
> Nearest neighbor matching selects for matching to a given treated subjectthat untreated subject whose propensity score is closest to that of the treatedsubject. If multiple untreated subjects have propensity scores that are equally close to that of the treated subject, one of these untreated subjects is selected at random. 

> [!quote|yellow]+ Highlight ([page. 9](zotero://open-pdf/library/items/DZ9UXJJD?page=9&annotation=XFWVIPUV))
> no restrictions are placed upon themaximum acceptable difference between the propensity scores of two matched subjects. 

> [!quote|yellow]+ Highlight ([page. 9](zotero://open-pdf/library/items/DZ9UXJJD?page=9&annotation=GL92ICYI))
> Thus, for a given treated subject, one wouldidentify all the untreated subjects whose propensity score lay within a specified distance of that of the treated subject. From this restricted set of untreated subjects, the untreated subject whose propensity score was closest to that of the treated subject would be selected for matching to this treated subject. Ifno untreated subjects had propensity scores that lay within the specified caliper distance of the propensity score of the treated subject, that treated subject would not be matched with any untreated subject. The unmatched treated subject would then be excluded from the resultant matched sample. 

> [!quote|yellow]+ Highlight ([page. 10](zotero://open-pdf/library/items/DZ9UXJJD?page=10&annotation=IH9QWBRN))
> In many-to-one (M:1) matching, M untreated subjects are matched to each treated subject 
> - **Many untreated to treated**

> [!quote|yellow]+ Highlight ([page. 10](zotero://open-pdf/library/items/DZ9UXJJD?page=10&annotation=IGY3JWGZ))
> They found that improved bias reduction was obtained when matching witha variable number of controls compared to matching with a fixed number ofcontrols 
> - **i.e. M falls into a range of values and isn't fixed**

> [!quote|yellow]+ Highlight ([page. 10](zotero://open-pdf/library/items/DZ9UXJJD?page=10&annotation=5M7SWN8H))
> Stratification on the propensity score involves stratifying subjects into mutually exclusive subsets based on their estimated propensity score 
> - **by**

> [!quote|yellow]+ Highlight ([page. 11](zotero://open-pdf/library/items/DZ9UXJJD?page=11&annotation=ZIIJVRG8))
> a set of quasi-RCT 
> - **each stratification can be seen as a mini instance of a RCT**

> [!quote|yellow]+ Highlight ([page. 11](zotero://open-pdf/library/items/DZ9UXJJD?page=11&annotation=SBZR6MLY))
> general, stratum-specific estimates of effect are weighted by the proportion of subjects who lie within that stratum. Thus, when the sample is stratified into K equal-size strata, stratum-specific weights of 1=K are commonly used when pooling the stratum-specific treatment effects, allowing one to estimate the ATE ( 
> - **Summing all treatment effects across multiple stratum, with the weights**

> [!quote|yellow]+ Highlight ([page. 11](zotero://open-pdf/library/items/DZ9UXJJD?page=11&annotation=EATCURTZ))
> use of stratum-specific weights thatare equal to that proportion of treated subjects that lie within each stratum allow one to estimate the ATT 
> - **weighting by treated/total in each stratum**

> [!quote|yellow]+ Highlight ([page. 11](zotero://open-pdf/library/items/DZ9UXJJD?page=11&annotation=DV39HXQP))
> IPTW is similar to the use of survey sampling weightsthat are used to weight survey samples so that they are representative of specificpopulations 

> [!quote|yellow]+ Highlight ([page. 12](zotero://open-pdf/library/items/DZ9UXJJD?page=12&annotation=Q98KR6HS))
> Furthermore, this method assumes that the nature of the relationship between the propensity score and the outcome has been correctly modeled. 

> [!quote|yellow]+ Highlight ([page. 14](zotero://open-pdf/library/items/DZ9UXJJD?page=14&annotation=KETCSWIT))
> An important component of any propensity score analysis is examining whether the propensity score model has been adequately specified 

> [!quote|yellow]+ Highlight ([page. 14](zotero://open-pdf/library/items/DZ9UXJJD?page=14&annotation=SB2BUU3I))
> Appropriate methods for assessing whether the propensity score model has been adequately specified involve examining whether the distribution of measured baseline covariates is similar between treated and untreated subjects with the same estimated propensity score. 

> [!quote|yellow]+ Highlight ([page. 14](zotero://open-pdf/library/items/DZ9UXJJD?page=14&annotation=LM582GPI))
> begin with a comparison of the means or medians of continuous covariates and the distribution of their categorical counterparts between treated and untreated subjects 

> [!quote|yellow]+ Highlight ([page. 15](zotero://open-pdf/library/items/DZ9UXJJD?page=15&annotation=HZCXZCQ9))
> standardized differ-ence compares the difference in means in units of 

> [!quote|yellow]+ Highlight ([page. 15](zotero://open-pdf/library/items/DZ9UXJJD?page=15&annotation=8F6HKN96))
> a standard differencethat is less than 0.1 has been taken to indicate a negligible difference in the meanor prevalence of a covariate between treatment groups ( 

> [!quote|yellow]+ Highlight ([page. 15](zotero://open-pdf/library/items/DZ9UXJJD?page=15&annotation=FREWSQKH))
> entire distribution of baseline covariates, not just means and prevalences, should be similar between treatment groups in the matched sample. 

> [!quote|yellow]+ Highlight ([page. 16](zotero://open-pdf/library/items/DZ9UXJJD?page=16&annotation=9698GWY9))
> statistical significance testing to com-pare the mean of continuous covariates or the distribution of categorical variables between treated and untreated subjects in propensity score matched samples 

> [!quote|yellow]+ Highlight ([page. 17](zotero://open-pdf/library/items/DZ9UXJJD?page=17&annotation=3VFAYFS9))
> there are theoretical arguments in favorof the inclusion of only those variables that affect treatment assignment. 

> [!quote|yellow]+ Highlight ([page. 18](zotero://open-pdf/library/items/DZ9UXJJD?page=18&annotation=RGRQE6BS))
> When only the potential confoundersor only the true confounders were included in the propensity score model, the variables that were imbalanced between treated and untreated subjects were those variables that affected treatment assignment but that were independentof the outcome. 

> [!quote|yellow]+ Highlight ([page. 18](zotero://open-pdf/library/items/DZ9UXJJD?page=18&annotation=Q33WYHWS))
> greater number of matched pairs were formed 

> [!quote|yellow]+ Highlight ([page. 18](zotero://open-pdf/library/items/DZ9UXJJD?page=18&annotation=MHACTK55))
> potential confounders or the true confounders)resulted in estimates of a null treatment effect that had lower mean squared erro 

> [!quote|yellow]+ Highlight ([page. 18](zotero://open-pdf/library/items/DZ9UXJJD?page=18&annotation=NURNGFDF))
> including variables that affect exposure but not the outcome willincrease the variance of the estimated treatment effect without a concomitant reduction in bias. 

> [!quote|yellow]+ Highlight ([page. 19](zotero://open-pdf/library/items/DZ9UXJJD?page=19&annotation=A8GWGDBC))
> observationalstudy in which (a) there was no unmeasured confounding, (b) the outcome was continuous, and (c) the true outcome model was known, the marginaland conditional estimates would coincide. 
> - **All confounders must be measured**

> [!quote|yellow]+ Highlight ([page. 20](zotero://open-pdf/library/items/DZ9UXJJD?page=20&annotation=DBXM8CLT))
> estimates obtained usingpropensity score methods tended to be modestly closer to the null compared with when regression-based approaches were used for estimating odds ratios orhazard ratios. 

> [!quote|yellow]+ Highlight ([page. 20](zotero://open-pdf/library/items/DZ9UXJJD?page=20&annotation=5S44LYKP))
> simpler to determine whether the propensityscore model has been adequately specified than to assess whether the regressionmodel relating treatment assignment and baseline covariates to the outcome hasbeen correctly specified 

> [!quote|yellow]+ Highlight ([page. 20](zotero://open-pdf/library/items/DZ9UXJJD?page=20&annotation=RZR7C3ZR))
> methods allow one to separate the design of the study from the analysis of the study. This is similar to an RCT, in which the study is designedfirst; 

> [!quote|yellow]+ Highlight ([page. 21](zotero://open-pdf/library/items/DZ9UXJJD?page=21&annotation=DLYTHD36))
> faced with the sparse overlap 

> [!quote|yellow]+ Highlight ([page. 21](zotero://open-pdf/library/items/DZ9UXJJD?page=21&annotation=4ATVGD76))
> When using regression-based approaches, it may be difficult to assess the degree of overlap between the distribution of baseline covariates for the two groups 

### 🔗 Interesting references

> [!quote|blue]+ Highlight ([page. 5](zotero://open-pdf/library/items/DZ9UXJJD?page=5&annotation=WJ965QSI))
> propensity score was defined by Rosenbaum and Rubin (1983a) to be the probability of treatment assignment conditional on observed baseline covariates: ei D P r .Zi D 1jXi/ 

> [!quote|blue]+ Highlight ([page. 5](zotero://open-pdf/library/items/DZ9UXJJD?page=5&annotation=ZID5MBHR))
> balancing score: conditional onthe propensity score, the distribution of measured baseline covariates is similar between treated and untreated subjects 

> [!quote|blue]+ Highlight ([page. 7](zotero://open-pdf/library/items/DZ9UXJJD?page=7&annotation=2MBD78SI))
> he most common implementation of propensity score matching is one-to-one or pair matching, in which pairs of treated and untreated subjects are formed, such that matched subjects have similar values of the propensity score. Although one-to-one matching appears to be the most common approac 

> [!quote|blue]+ Highlight ([page. 10](zotero://open-pdf/library/items/DZ9UXJJD?page=10&annotation=WNNDHIF7))
> Full matching (Gu & Rosenbaum, 1993; Hansen, 2004; Rosenbaum, 1991) involves forming matched sets consisting of either one treated subject andat least one untreated subject or one untreated subject and at least one treatedsubject. 
> - **read up**

> [!quote|blue]+ Highlight ([page. 14](zotero://open-pdf/library/items/DZ9UXJJD?page=14&annotation=4JAYTBSQ))
> true propensity score is a balancing score: conditional on the true propensity score, the distribution of measured baseline covariates is independent of treatment assignment 

> [!quote|blue]+ Highlight ([page. 14](zotero://open-pdf/library/items/DZ9UXJJD?page=14&annotation=V55E6KKU))
> I summarize an extensive previous discussion of methods forassessing the comparability of treated and untreated subjects in a propensity score matched sample (Austin, 2009b). The methods described are for use inthe context of one-to-one matching on the propensity score. Adaptations for use with many-to-one matching on the propensity score are provided elsewhere (Austin, 2008d). 

> [!quote|blue]+ Highlight ([page. 19](zotero://open-pdf/library/items/DZ9UXJJD?page=19&annotation=X7GX5ARJ))
> A conditional treatment effect is the average effect of treatment on the individual.<br />
A marginal treatment effect is the average effect of treatment on the population. 

> [!quote|blue]+ Highlight ([page. 19](zotero://open-pdf/library/items/DZ9UXJJD?page=19&annotation=QND2CQKU))
> when the outcome is either binary or time-to-event in nature and ifthe odds ratio or the hazard ratio is used as the measure of treatment effect, then,even in the absence of confounding, the marginal and conditional estimates of the treatment effect need not coincide (Gail, Wieand, & Piantadosi, 1984; Greenland, 1987) 

### 🧩 Methodology

> [!quote|purple]+ Highlight ([page. 400](zotero://open-pdf/library/items/DZ9UXJJD?page=400&annotation=6LY4MDQP))
> Historically, applied researchers have relied on the use of regression adjustment to account for differences in measured baseline characteristics between treated and untreated subjects. Recently, there has been increasing interest in methods based on the propensity score 
> - **differences??**

> [!quote|purple]+ Highlight ([page. 400](zotero://open-pdf/library/items/DZ9UXJJD?page=400&annotation=PPF43V5Z))
> first, I briefly describe the potential outcomes framework, causal treatment effects, RCTs, and observational studies. Second, I introduce the concept of the propensity score and describe four different methods in which it can be used to estimate treatment effects. Third, I describe methods to assess whether the propensity score model has been adequately specified. Fourth, I discuss variable selection for the propensity score model. Fifth, I compare the use of propensity scorebased approaches with that of regression analyses in observational studies. Sixth, I summarize our discussion in the final section. 
> - **outline**

> [!quote|purple]+ Highlight ([page. 6](zotero://open-pdf/library/items/DZ9UXJJD?page=6&annotation=GVIYLBP7))
> In practice, the propensity score is most often estimated using a logistic regression model, in which treatment status is regressed on observed baseline characteristics. 

> [!quote|purple]+ Highlight ([page. 6](zotero://open-pdf/library/items/DZ9UXJJD?page=6&annotation=KPTDHJ9F))
> estimated propensity score is the predicted probability oftreatment derived from the fitted regression model 

> [!quote|purple]+ Highlight ([page. 8](zotero://open-pdf/library/items/DZ9UXJJD?page=8&annotation=KRPFQI6D))
> different methods for forming matched pairs of treated anduntreated subjects when matching on the propensity score 

> [!quote|purple]+ Highlight ([page. 8](zotero://open-pdf/library/items/DZ9UXJJD?page=8&annotation=3L5TUS8N))
> one must choose between matching withoutreplacement and matching with replacement (Rosenbaum, 2002) 

> [!quote|purple]+ Highlight ([page. 8](zotero://open-pdf/library/items/DZ9UXJJD?page=8&annotation=UE8ZTQT9))
> greedy matching, a treated subject is first selected at random. The untreated subject whose propensity score is closest to that of this randomly selected treated subject is chosen for matching to this treated subject. This process is then repeated until untreated subjects have been matched to all treated subjects or until one has exhausted the list of treated subjects for whom a matched untreated subject can be found 

> [!quote|purple]+ Highlight ([page. 9](zotero://open-pdf/library/items/DZ9UXJJD?page=9&annotation=MMW4YJ3X))
> selectinguntreated subjects whose propensity score is “close” to that of a treated subject.  There are two primary methods for this: nearest neighbor matching and nearestneighbor matching within a specified caliper distance 

> [!quote|purple]+ Highlight ([page. 10](zotero://open-pdf/library/items/DZ9UXJJD?page=10&annotation=BREW348R))
> It was suggested that researchers use a caliper of widthequal to 0.2 of the standard deviation of the logit of the propensity score as this value (or one close to it) minimized the mean squared error of the estimated treatment effect in several scenarios. 

> [!quote|purple]+ Highlight ([page. 10](zotero://open-pdf/library/items/DZ9UXJJD?page=10&annotation=LBNCGYR6))
> A common approach is to divide subjects into five equal-size groups using the quintiles of the estimated propensity score 
> - **can also stratify on the quintiles of the confounder if it is continuous**

> [!quote|purple]+ Highlight ([page. 11](zotero://open-pdf/library/items/DZ9UXJJD?page=11&annotation=FH74T2YK))
> let Zi be an indicator variable denoting whether or notthe ith subject was treated; furthermore, let ei denote the propensity score for the ith subject. Weights can be defined as wi D ZieiC .1 Zi/ 1 e 

> [!quote|purple]+ Image ([page. 15](zotero://open-pdf/library/items/DZ9UXJJD?page=15&annotation=HJ22YDAU))
> ![[30 Resources/39 Literature Notes/@austin_2011/@austin_2011-15-x29-y489.png]]

> [!quote|purple]+ Image ([page. 15](zotero://open-pdf/library/items/DZ9UXJJD?page=15&annotation=BJE886IQ))
> ![[30 Resources/39 Literature Notes/@austin_2011/@austin_2011-15-x46-y383.png]]

> [!quote|purple]+ Highlight ([page. 17](zotero://open-pdf/library/items/DZ9UXJJD?page=17&annotation=PDUH8DFJ))
> VARIABLE SELECTION FOR THE PROPENSITYSCORE MODEL 

> [!quote|purple]+ Highlight ([page. 17](zotero://open-pdf/library/items/DZ9UXJJD?page=17&annotation=N3HJ2P3C))
> all measured baselinecovariates, all baseline covariates that are associated with treatment assignment, all covariates that affect the outcome (i.e., the potential confounders), and all covariates that affect both treatment assignment and the outcome 

> [!quote|purple]+ Highlight ([page. 17](zotero://open-pdf/library/items/DZ9UXJJD?page=17&annotation=U9SV6JGE))
> meritsto including only the potential confounders or the true confounders in thepropensity score model. 
%% end annotations %%

%% Import Date: 2025-07-19T15:08:01.832+08:00 %%
