```dataview  
TABLE  
title as Title,  
itemType as Item,  
status as Status,  
dateread as Read,  
contribution as Contribution  
WHERE contains(tags, "JACSIS2023_Vaccine_Uptake")  
SORT status DESC, read DESC  
```

This is a table to show all the papers that you've shortlisted to be cited, and their respective contributions. To include a paper in this table, just add #[insert your project name here] to the tags field of the respective literature note you want to cite

and make sure to change the tag you look for in the dataview snippet above

