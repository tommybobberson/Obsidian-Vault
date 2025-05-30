---
category: literaturenote
aliases:
tags: {% if allTags %}{{allTags}}{% endif %}
citekey: {{citekey}}
doi: {{DOI}}
status: unread
dateread: 
---
# [{{title}}]({{desktopURI}})
> [!Cite]
> {% if bibliography %}{{bibliography|replace("\n"," ")}}{% endif %}

>[!Synth]  
>**Contribution**::  
>  
>**Related**:: {% if relations %}
>{% for relation in relations %} [[@{{ relation.citekey }}]]{% if not loop.last %}, {% endif %}{% endfor %}
>{% else %}
>No related literature found.
>{% endif %}


>[!md]
{% for type, creators in creators | groupby("creatorType") -%}
{%- for creator in creators -%}
> **{{"First" if loop.first}}{{type | capitalize}}**::
{%- if creator.name %} {{creator.name}}  
{%- else %} {{creator.lastName}}, {{creator.firstName}}  
{%- endif %}  
{% endfor %}~ 
{%- endfor %}    
> **Title**:: {{title}}  
> **Year**:: {{date | format("YYYY")}}   
> **Citekey**:: {{citekey}} {%- if itemType %}  
> **itemType**:: {{itemType}}{%- endif %}{%- if itemType == "journalArticle" %}  
> **Journal**:: *{{publicationTitle}}* {%- endif %}{%- if volume %}  
> **Volume**:: {{volume}} {%- endif %}{%- if issue %}  
> **Issue**:: {{issue}} {%- endif %}{%- if itemType == "bookSection" %}  
> **Book**:: {{publicationTitle}} {%- endif %}{%- if publisher %}  
> **Publisher**:: {{publisher}} {%- endif %}{%- if place %}  
> **Location**:: {{place}} {%- endif %}{%- if pages %}   
> **Pages**:: {{pages}} {%- endif %}{%- if DOI %}  
> **DOI**:: {{DOI}} {%- endif %}{%- if ISBN %}  
> **ISBN**:: {{ISBN}} {%- endif %}    

> [!LINK] 
> {%- for attachment in attachments | filterby("path", "endswith", ".pdf") %}
>  [{{attachment.title}}](file://{{attachment.path | replace(" ", "%20")}})  {%- endfor -%}.

> [!Abstract]
> {%- if abstractNote %}
> {{abstractNote}}
> {%- endif -%}.
> 

--- 
{% persist "notes" %}{% if isFirstImport %}
## Main ideas:
- 
## Methodology:
- 
## Results:
- 
## Key points:
- 
{% endif %}{% endpersist %}
## Reading notes
{% persist "annotations" %}
{%-
    set zoteroColors = {
        "#ff6666": "red",
        "#f19837": "orange",
        "#5fb236": "green",
        "#ffd400": "yellow",
        "#2ea8e5": "blue",
        "#a28ae5": "purple",
        "#e56eee": "magenta",
        "#aaaaaa": "grey"
    }
-%}

{%-
   set colorHeading = {
		"red": "⭕ Very important or questionable",
		"orange": "⭐ Important or interesting",
		"green": "✅ Major statements",
		"yellow": "📚 Ordinary notes",
        "blue": "🔗 Interesting references",
        "purple": "🧩 Methodology",
        "other": "Misc"
   }
-%}

{%- macro calloutHeader(type) -%}
    {%- switch type -%}
        {%- case "highlight" -%}
        Highlight
        {%- case "image" -%}
        Image
        {%- default -%}
        Note
    {%- endswitch -%}
{%- endmacro %}

{%- set newAnnot = [] -%}
{%- set newAnnotations = [] -%}
{%- set annotations = annotations | filterby("date", "dateafter", lastImportDate) %}

{% if annotations.length > 0 %}
*Imported: {{importDate | format("YYYY-MM-DD HH:mm")}}*

{%- for annot in annotations -%}

    {%- if annot.color in zoteroColors -%}
        {%- set customColor = zoteroColors[annot.color] -%}
    {%- elif annot.colorCategory|lower in colorHeading -%}
    	{%- set customColor = annot.colorCategory|lower -%}
    {%- else -%}
	    {%- set customColor = "other" -%}
    {%- endif -%}

    {%- set newAnnotations = (newAnnotations.push({"annotation": annot, "customColor": customColor}), newAnnotations) -%}

{%- endfor -%}

{#- INSERT ANNOTATIONS -#}
{#- Loops through each of the available colors and only inserts matching annotations -#}
{#- This is a workaround for inserting categories in a predefined order (instead of using groupby & the order in which they appear in the PDF) -#}

{%- for color, heading in colorHeading -%}
{%- for entry in newAnnotations | filterby ("customColor", "startswith", color) -%}
{%- set annot = entry.annotation -%}

{%- if entry and loop.first %}

### {{colorHeading[color]}}
{%- endif %}

> [!quote{{"|" + color if color != "other"}}]+ {{calloutHeader(annot.type)}} ([page. {{annot.pageLabel}}](zotero://open-pdf/library/items/{{annot.attachment.itemKey}}?page={{annot.pageLabel}}&annotation={{annot.id}}))

{%- if annot.annotatedText %}
> {{annot.annotatedText|nl2br}} {% if annot.hashTags %}{{annot.hashTags}}{% endif -%}
{%- endif %}

{%- if annot.imageRelativePath %}
> ![[{{annot.imageRelativePath}}]]
{%- endif %}

{%- if annot.ocrText %}
> {{annot.ocrText}}
{%- endif %}

{%- if annot.comment %}
> - **{{annot.comment|nl2br}}**
{%- endif -%}

{%- endfor -%}
{%- endfor -%}
{% endif %}
{% endpersist -%}