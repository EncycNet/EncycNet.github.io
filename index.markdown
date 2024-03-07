---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: EncycNet Project
---

**EncycNet**, funded by the German Research Foundation (DFG) and begun in 2019, aims to
create a new semantic resource for historical German in the form of a richly annotated knowledge graph (a nodes and edges network). By linking the knowledge contained within thousands of encyclopedia entries via machine learning classification and semantic web annotation, EncycNet provides a unique resource for a variety of historical, cultural, and computational linguistic research goals.  
  
    

<img src="EncycNet website image top.jpg" alt="EncycNet - Knowledge Graph" width="900" align="center" style="margin-top: 60px"/>  

<p style="color:grey; margin-bottom: 60px; margin-left: 60px; margin-top: -20px; font-size: 10px; text-align: left"><a href="https://fr.wikipedia.org/wiki/Fichier:2020_11_04_004_Meyers_Konversations_Lexikon.jpg" style="color: #D5D5D5;
  background-color: transparent;">Creative Commons</a></p>


### Publications and presentations

- Thora Hagen, Fotis Jannidis and Andreas Witt, “Mental Maps in EncycNet: Exploring Global Representation in a Historical, German Knowledge Graph, DH2024, August 2024 (accepted).
- Thora Hagen, Leonard Konle, Erik Ketzan, Fotis Jannidis and Andreas Witt, [“Tracing the Shift to 'Objectivity' in German Encyclopedias of the Long Nineteenth Century”](https://zenodo.org/records/8107633), DH2023, July 2023.
- Thora Hagen, [“EncycNet: Graphen-basierte Modellierung von historischem, enzyklopädischem Wissen”](https://dhistory.hypotheses.org/5715), Forschungskolloquium 'Digital History', June 2023.
- Thora Hagen, [“Von A bis Z: Überlegungen zur Erstellung eines Wissensgraphen aus historischen Enzyklopädien”](https://zenodo.org/records/7715341), DHd 2023: 9. Tagung des Verbands 'Digital Humanities im deutschsprachigen Raum', March 2023.
- Erik Ketzan, Thora Hagen, Fotis Jannidis and Andreas Witt, [“Quantitative Analysis of Gendered Assumptions in a Nineteenth-Century Women’s Encyclopedia”](https://www.erikketzan.com/wp-content/uploads/2022/08/Ketzan_et_al_Gendered_Assumptions.pdf), DH2022, July 2022. 
- Andreas Witt, Thora Hagen and Fotis Jannidis, “Introducing EncycNet: Graph-based Modeling of 19th Century German Encyclopedic Knowledge”, 5th Annual GHI Conference on Digital Humanities and Digital History, June 2022.
- Thora Hagen, Fotis Jannidis and Andreas Witt, [“Word Sense Alignment and Disambiguation for Historical Encyclopedias“](https://graphentechnologien.hypotheses.org/files/2022/01/Word_Sense_Alignment_and_Disambiguation_for_Historical_etc-Hagen_Jannidis_Witt.pdf), 6th international conference on Graphs and Networks in the Humanities, February 2022.
- Thora Hagen, Erik Ketzan, Fotis Jannidis and Andreas Witt, [“Twenty-Two Historical Encyclopedias Encoded in TEI: A New Resource for the Digital Humanities”](https://www.aclweb.org/anthology/2020.latechclfl-1.13.pdf), LaTeCH-CLfL 2020: 4th Joint SIGHUM Workshop on Computational Linguistics for Cultural Heritage, Social Sciences, Humanities and Literature, December 2020.

### Data

- [TEI-transformed corpus and ODD](http://dx.doi.org/10.5281/zenodo.4039569)
- [Original XML corpus](http://dx.doi.org/10.5281/zenodo.4159491)
- [TEI transformation with XSLT](https://github.com/EncycNet/Encyc-Transformation)
- [CSV data of Wikidata alignment and relation extraction](https://github.com/EncycNet/Encyc-Relations) (work in progress)
- [Application for data exploration, including Wikidata alignment](http://encycnet.digital-humanities.de)
- [EncycNet Knowledge Graph (RDF)](http://dx.doi.org/10.5281/zenodo.10219192) (currently contains Meyers 1905, work in progress)

### What we have done so far

- ingested 22 historical German encyclopedias from the early 18th to early 20th century, over 49,300,000 word tokens, in XML format, provided by [TextGrid](https://textgrid.de) and [Zeno.org](http://www.zeno.org)
- transformed the corpus to TEI Lex-0, to unify and disambiguate the original XML encoding, and to suggest changes to  TEI methodology for  encyclopedic texts
- published the TEI corpus and transformation code
- performed corpus annotation including Part-of-Speech tagging, lemmatization, orthographic normalization (see Acknowledgements, below) as well as Named Entity Recognition and transformed the TEI to CSV files
- developed Hearst patterns (defined as lexico-syntactic recognition of hyponymy; but for EncycNet, several relation types are of importance) from the encyclopedia texts to aid with triple extraction

### Ongoing steps

- splitting encyclopedia entries that contain multiple concepts
- creating a list of concepts from the encyclopedia entries by linking the entries to Wikipedia pages (including semantic disambiguation)
- linking the concepts to hypernyms using Wikidata
- extracting triples from the encyclopedia entries by utilizing explicitly annotated references, Hearst patterns and typography tags in general

The EncycNet knowledge graph also aims to meet the following requirements: each triple can be traced back to its origin so that temporal information will be retained. As the triples will be extracted automatically, each triple will also be annotated with a confidence score. The graph will be linked to Wikipedia and the GND and can potentially be connected to other Linked Open Data resources as well. Lastly, tutorials for different use cases will be made available in the future to demonstrate how to work with EncycNet, with special attention to improving word embeddings with newfound historical-semantic knowledge.
  
## Team

- [Fotis Jannidis](http://www.jannidis.de), University of Würzburg
- [Andreas Witt](https://www1.ids-mannheim.de/digspra/personal/witt.html), IDS Mannheim & University of Cologne
- Thora Hagen, University of Würzburg
- [Erik Ketzan](https://www.erikketzan.com), University of Cologne (July 2020 - Sept. 2021)

## Research assistants

- Corinna Keupp
- Maximilian Supplieth
- Nicolas Werner (April 2021 - Sept. 2021)


## Contact

Thora Hagen

<thora.hagen@uni-wuerzburg.de>

### Acknowledgements

Thanks to the German Text Archive (Deutsches Textarchiv), especially Bryan Jurish, who
generously performed the orthographic normalization, lemmatization and Part-of-Speech tagging of all encyclopedia texts using [CAB](https://kaskade.dwds.de/~moocow/software/DTA-CAB/doc/html/DTA.CAB.WebServiceHowto.html).
