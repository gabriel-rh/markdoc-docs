# test markdoc features


## code block

{% code %}

some code herr

{% /code %}

## Side by side test
{% sidebyside %}

{% item %}

- list item 1 here
- list item 2 here

```
puts "Some code here."
```

{% /item %}

{% item %}

{% table %}
* Heading 1
* Heading 2
---
* Row 1 Cell 1
* Row 1 Cell 2
---
* Row 2 Cell 1
* Row 2 cell 2
{% /table %}

{% /item %}


{% /sidebyside %}


## Nested tables


{% table %}
* Heading 1
* Heading 2
* Heading 3
---
* Row 1 Cell 1
* Row 1 cell 2
* Row 1 cell 3
---
* Row 2 cell 1 
*
  {% table %}
  * nested Heading 1
  * nested Heading 2
  ---
  * nested Row 1 Cell 1
  * nested Row 1 Cell 2
  ---
  * nested Row 2 Cell 1
  * nested Row 2 cell 2
  {% /table %}
* Row 2 Cell 3
---
* Row 3 Cell 1
* Row 3 cell 2
* Row 3 cell 3
{% /table %}


## Paritals test

{% partial file="header.md" /%}

{% partial file="proc_creating-a-git-repository.md" /%}