# NLP parser

Basic probabilistic parser for French based on the CYK algorithm and the PCFG model. First a module extracts the grammar from bracketed sentences (with the help of [NLTK](https://www.nltk.org/)) then we parse new sentences (after training the model on the first 80% sentences). To handle out of vocabulary we use a combination of [cosine similarity](https://en.wikipedia.org/wiki/Cosine_similarity) and [Damereau Levenshtein distance](https://en.wikipedia.org/wiki/Damerau%E2%80%93Levenshtein_distance). 

N.b.: one must first unzip the file `polyglot-fr.pkl`.
