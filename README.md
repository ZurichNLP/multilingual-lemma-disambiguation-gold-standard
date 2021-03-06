# Readme
The goldstandards contain words with ambiguous lemmatizations generated by the TreeTagger. The words are taken from sentences from the Europarl Corpus.

## File Types

The goldstandard\*0s.tsv files contain 100 ambiguous lemmatizations with one or no unambiguous lemma candidate in FEP6. They have been used to evaluate the active learning approach as described in the Thesis. The other files contain a varying amount of ambiguous lemmatizations with unambiguous evidence for both lemmas in FEP6.

## Format
The goldstandard uses a simple tabulator-separated textual data format. The meaning of the columns is as follows:

 1. ID of token in the FEP6 corpus
 2. word form of ambiguous token
 3. ambiguous lemmatization candidates (pipe-separated)
 4. gold lemma 
 5. part of the sample sentence before the ambiguous token
 6. word form of the ambiguous token
 7. part of the sample sentence after the ambiguous token.

Note that in rare cases the gold lemma might not be contained in the lemmatization candidate list, which is taken from the TreeTagger output. 
The sample sentences are tokenized such that each token is separated by a whitespace character.
