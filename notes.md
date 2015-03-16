class: center, middle
#Information Retrieval Based on Word Sense

---

#Roadmap
- Word sense and it's role in ambiguity
- Word sense in a standard IR system
- Existing approaches to automatic word sense disambiguation
- New idea: constructing a thesaurus from the existing corpus for word sense disambiguation
	- Use a vector representation for word similarity derived from lexical co-occurrence in the corpus text
- Performance of this algorithm in an IR system 

---

#Introduction - Word Sense
- Ambiguous term: **a word with multiple senses, where a sense is a group of similar usages of a word dissimilar from other usages**
	
	- homographs 
		- words sharing the same written form but having different meaning
		- "river bank" vs. "Bank of New York"
	- graded sense
		 - words sharing the same written form and general meaning but having different meaning depending on context
		- "line space" vs. "office space" vs. "exhibition space"
	
	
---

class: center, middle
	![Bass Fishing Area](images/bass-fishing-area.jpg)

---

#Introduction - Determining Word Sense

- What do we use to determine the sense of a word?

	- syntactic role
		- functional relationship between the word and other words in a clause
	- nearby words
		- provide cues and context for the words
	- semantics
		- our own general understanding of the meaning
		
- Without **context**, it is impossible to determine sense

---

#Introduction - Ambiguous Terms in IR

- In the bag of words approach, each word is treated as a separate isolated feature
	- __Context is not preserved__
	- Disambiguating word sense is not explicitly achieved
	
-  *However*, since retrievals rarely depend on a single term, it is often the case that implicit disambiguation of a word sense is achieved
	- Documents are retrieved by matching many of the query terms
	
-  Nonetheless, **word sense disambiguation algorithms** should help
	- Should not decrease performance of a standard IR
	- Should increase performance on shorter queries that will provide less opportunity for implicit disambiguation

---

#Existing Approaches
- Hand constructed disambiguation rules & hand labeled training sets
	- Providing the system with pre-defined sets of rules or training data to disambiguate words with multiple senses
	- Problem: lots of manual effort required for construction
	
- Online dictionaries

- Constructed knowledge bases


- Computation based on Roget's thesaurus
	- Determining the similarity of an ambiguous word to other words using a thesaurus

???

- Syntactic and semantic structure in a connectionist set
	-

- Online dictionaries

---

#Existing Approaches - Common Problems

- **Lack of coverage**

	 - Specialized domains have corpus text containing rare words with specialized meaning that is not covered by generic lexical resources
	 
	 - Cost of customizing the resources to accomodate specialized domains is high

- 
---

#Wordnet Thesaurus
- WordNet:  It groups English words into sets of synonyms called synsets
	- Transformed into a mapping from words to one or more classes
	
---
	
#Novel Approach: Thesaurus Construction

asdf
asdfdw
sadfasdf
asdfasd

---

#MISC
Semantic similarity or semantic relatedness is a metric defined over a set of documents or terms, where the idea of distance between them is based on the likeness of their meaning or semantic content as opposed to similarity which can be estimated regarding their syntactical representation (e.g. their string format). 

Main problem: lack of coverage; specific corpus have highly specialized terms that often are not covered in general thesaurus's like wordnet