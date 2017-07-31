<a href="http://data.cervantesvirtual.com/"><img src=http://data.cervantesvirtual.com/blog/wp-content/uploads/2017/05/fbvmc.png></a> 

# ner-corpora
Named Entity Recognition data for [Biblioteca Virtual Miguel de Cervantes](http://data.cervantesvirtual.com)

### Introduction
The corpora comprise files encoded in the BIO format (Ramshaw & Marcus, 1995). The BIO format is a simple, text-based format that divides texts into single tokens per line, and, separated by a whitespace, tags to indicate which ones are named entities. The most commonly used tags are *PER* (person), *LOC* (location) and *ORG* (organization). *O* tags are used to indicate that the token is not a named entity.

Example:
```
En	O
Valladolid	LOC
,	O
en	O
la	O
Imprenta	O
de	O
Alonso	PERS
del	PERS
Riego	PERS
...	O
,	O
-LSB-	O
s.a.	O
-RSB-	O
Impressa	O
en	O
Valladolid	LOC
,	O
en	O
la	O
Imprenta	O
de	O
Alonso	PERS
del	PERS
Riego	PERS
```

### License
[CC0](https://creativecommons.org/publicdomain/zero/1.0/)

You are free to use this data without restrictions. We're thankful if you give attribution to:

*Biblioteca Virtual Miguel de Cervantes NER corpora*   
*https://github.com/fbvmc/ner-corpora/.*  
*http://data.cervantesvirtual.com/.*

[Semantic Enrichment on Cultural Heritage collections: A case study using geographic information. Gustavo Candela, Pilar Escobar, Manuel Marco-Such](http://dl.acm.org/citation.cfm?doid=3078081.3078090)

### Background
The way the above corpora were produced, additional work is required to harness the full potential of the annotated data for tasks such as evaluation, where gold standard quality is required. Currently, the corpora has been mainly annotated with locations. Further work is needed in order to take advantage of Persons and Organizations.
Based on the BIO  files classifiers for the Stanford NER Recognizer were trained and subsequently evaluated in a 4-fold cross-evaluation. The files can be found in [cross-validation](cross-validation) folder.

