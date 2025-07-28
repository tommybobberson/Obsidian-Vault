---
category: literaturenote
aliases:
tags: methodology, causal inference
citekey: nilsson_2020
doi: 10.1093/ije/dyaa211
status: unread
dateread: 
---
# [A directed acyclic graph for interactions](zotero://select/library/items/PN8R444C)
> [!Cite]
> 1  Nilsson A, Bonander C, Strömberg U, Björk J. A directed acyclic graph for interactions. _Int J Epidemiol_ 2020;**50**:613–9. [https://doi.org/10.1093/ije/dyaa211](https://doi.org/10.1093/ije/dyaa211).

>[!Synth]  
>**Contribution**::  
>  
>**Related**:: 
>
>


>[!md]
> **FirstAuthor**:: Nilsson, Anton  
> **Author**:: Bonander, Carl  
> **Author**:: Strömberg, Ulf  
> **Author**:: Björk, Jonas  
~    
> **Title**:: A directed acyclic graph for interactions  
> **Year**:: 2020   
> **Citekey**:: nilsson_2020  
> **itemType**:: journalArticle  
> **Journal**:: *International Journal of Epidemiology*  
> **Volume**:: 50  
> **Issue**:: 2   
> **Pages**:: 613-619  
> **DOI**:: 10.1093/ije/dyaa211    

> [!LINK] 
>
>  [Nilsson et al. - 2020 - A directed acyclic graph for interactions.pdf](file://G:\My%20Drive\Work\Zotero\Nilsson%20et%20al.%20-%202020%20-%20A%20directed%20acyclic%20graph%20for%20interactions.pdf).

> [!Abstract]
>
> Background
Directed acyclic graphs (DAGs) are of great help when researchers try to understand the nature of causal relationships and the consequences of conditioning on different variables. One fundamental feature of causal relations that has not been incorporated into the standard DAG framework is interaction, i.e. when the effect of one variable (on a chosen scale) depends on the value that another variable is set to. In this paper, we propose a new type of DAG—the interaction DAG (IDAG), which can be used to understand this phenomenon.

Methods
The IDAG works like any DAG but instead of including a node for the outcome, it includes a node for a causal effect. We introduce concepts such as confounded interaction and total, direct and indirect interaction, showing that these can be depicted in ways analogous to how similar concepts are depicted in standard DAGs. This also allows for conclusions on which treatment interactions to account for empirically. Moreover, since generalizability can be compromised in the presence of underlying interactions, the framework can be used to illustrate threats to generalizability and to identify variables to account for in order to make results valid for the target population.

Conclusions
The IDAG allows for a both intuitive and stringent way of illustrating interactions. It helps to distinguish between causal and non-causal mechanisms behind effect variation. Conclusions about how to empirically estimate interactions can be drawn—as well as conclusions about how to achieve generalizability in contexts where interest lies in estimating an overall effect.
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


*Imported: 2025-06-05 22:55*

### ⭐ Important or interesting

> [!quote|orange]+ Highlight ([page. 614](zotero://open-pdf/library/items/4MGTJ3XA?page=614&annotation=5GSIBDMX))
> Key Messages  • Directed acyclic graphs (DAGs) are useful in epidemiology, but the standard framework offers no way of displaying  whether interactions are present (on the scale of interest).  • We present a new type of DAG—the interaction DAG (IDAG)—which can be used to analyse interactions.  • We define concepts such as confounded interaction and total, direct and indirect interaction, and show how these  can easily be displayed with the IDAG.  • An applied researcher can use the IDAG to determine which treatment interactions to account for empirically.  • The IDAG can also be used to shed light on mechanisms that compromise generalizability and to determine which  variables to account for in order to make results valid for the target population. 

> [!quote|orange]+ Highlight ([page. 618](zotero://open-pdf/library/items/4MGTJ3XA?page=618&annotation=Z8HCZT3W))
> Whereas standard DAGs are nonparametric, we note that the IDAG is parametric in the sense that the absence of an interaction corresponds to a choice of functional form. This makes the IDAG somewhat less general than the standard DAG 

> [!quote|orange]+ Highlight ([page. 618](zotero://open-pdf/library/items/4MGTJ3XA?page=618&annotation=WZ4EVQU5))
> However, a functional form is inevitably imposed when conducting (parametric) estimation, and we believe it is rather an advantage that the IDAG narrows the gap between theory and estimation. As for any DAG, assumptions on how the variables in the IDAG are related must be made based on previous evidence 

### 📚 Ordinary notes

> [!quote|yellow]+ Highlight ([page. 614](zotero://open-pdf/library/items/4MGTJ3XA?page=614&annotation=JKDAN4PA))
> instead of depicting how different variables influence the outcome, the IDAG depicts how different variables influence the size of a chosen effect measure 

> [!quote|yellow]+ Highlight ([page. 615](zotero://open-pdf/library/items/4MGTJ3XA?page=615&annotation=KHKR7D6J))
> Like any DAG, the IDAG will normally be drawn based on previous literature, which in the case of the IDAG will have to include evidence on which treatment interactions are present 

> [!quote|yellow]+ Highlight ([page. 615](zotero://open-pdf/library/items/4MGTJ3XA?page=615&annotation=8PJN6CR3))
> Whether an interaction is present may depend on the scale and, in fact, two variables that influence an outcome will always interact on some scales 
> - **Where additive interactions may not be present but multiplicative interactions are?**

> [!quote|yellow]+ Highlight ([page. 615](zotero://open-pdf/library/items/4MGTJ3XA?page=615&annotation=7P7MA62E))
> On the other hand, there can be no arrow from Q to DYA in the IDAG unless Q points to Y in the standard DAG. This follows because the treatment effect depends on the outcomes, so only if a variable directly influences the outcomes may it also directly influence the effect size. 

> [!quote|yellow]+ Image ([page. 616](zotero://open-pdf/library/items/4MGTJ3XA?page=616&annotation=E6LI8URE))
> ![[30 Resources/39 Literature Notes/@nilsson_2020/@nilsson_2020-4-x47-y634.png]]
> - **(a) classic DAG, (b) IDAG showing an interaction effect of Q on A -> Y, (c) Q has no interaction effect of A -> Y**

### 🔗 Interesting references

> [!quote|blue]+ Highlight ([page. 615](zotero://open-pdf/library/items/4MGTJ3XA?page=615&annotation=DVNR9I5C))
> The phenomenon has been referred to as ‘effect modification by proxy 
> - **read up on this?**

### 🧩 Methodology

> [!quote|purple]+ Highlight ([page. 614](zotero://open-pdf/library/items/4MGTJ3XA?page=614&annotation=THNE5HQD))
> the general idea behind interaction is that the effect of one variable (on some scale) depends on the level to which another variable is set 
> - **their definition of an interaction**

> [!quote|purple]+ Image ([page. 614](zotero://open-pdf/library/items/4MGTJ3XA?page=614&annotation=SAQLVDW8))
> ![[30 Resources/39 Literature Notes/@nilsson_2020/@nilsson_2020-2-x328-y333.png]]
> - **definition of interaction, where a is the independent var of interest and q is the covariate**

> [!quote|purple]+ Highlight ([page. 614](zotero://open-pdf/library/items/4MGTJ3XA?page=614&annotation=SUNBYWQH))
> Interaction between Q and A is thus present if the size of this causal effect depends on Q. 

> [!quote|purple]+ Highlight ([page. 615](zotero://open-pdf/library/items/4MGTJ3XA?page=615&annotation=WY8GUHL6))
> For simplicity, we will assume that there are no interactions not involving A (on the chosen scale), and for this reason we only consider DYA and not, for example, DYQ 
%% end annotations %%

%% Import Date: 2025-06-05T22:56:01.811+08:00 %%
