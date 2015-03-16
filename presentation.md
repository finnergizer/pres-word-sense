class: center, middle
#Information Retrieval Based on Word Sense

---

#Roadmap
- Word sense and it's role in ambiguity
- Word sense in a standard IR system
- Existing approaches to automatic word sense disambiguation
- New idea: constructing a thesaurus from the existing corpus for word sense disambiguation
	- Use a vector representation for word similarity derived from lexical co-occurrence in the corpus
- Performance of this algorithm in an IR system 

---

#Introduction - Word Sense
- Ambiguous term: **a word with multiple senses, where a sense is a group of similar usages of a word dissimilar from other usages**
	- homographs
		- words sharing the same written form but having different meaning
		- "river bank" vs. "Bank of New Youk"
	- graded sense: 
		- words sharing the same written form and general meaning but having different meaning depending on context
		- "line space" vs. "office space" vs. "exhibition space"

- What do we use to determine sense?
	- syntactic role
	- nearby words
	- semantics

- Without __**context**__, it is impossible to determine which sense

--

#Ambiguous Terms in IR
- In the bag of words approach, each word is treated as a separate isolated feature
	-  __context is not preserved__
-  *Note: Even though context is not explicitly preserved, since retrievals rarely depend on a single term, it is often the case that appropriate documents are retrieved using the set of related terms.*
-  Solution: word sense disambiguation algorithms
	-  Should not decrease performance
---
#Related Work
- Hand constructed disambiguation rules
- Online dictionaries
- Constructed knowledge bases
- Syntactic and semantic structure in a connectionist set
- Hand-labeled training sets
- Computation based on Roget's thesaurus
---
#Wordnet Thesaurus
- WordNet:  It groups English words into sets of synonyms called synsets
	- Transformed into a mapping from words to one or more classes
	- Syntactic and semantic structure in a connectionist set
	- Hand-labeled training sets

---


---
#MISC
Semantic similarity or semantic relatedness is a metric defined over a set of documents or terms, where the idea of distance between them is based on the likeness of their meaning or semantic content as opposed to similarity which can be estimated regarding their syntactical representation (e.g. their string format). 