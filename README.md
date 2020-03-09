# NLP parser

Basic probabilistic parser for French based on the CYK algorithm and the PCFG model. First a module extracts the grammar from bracketed sentences (with the help of [NLTK](https://www.nltk.org/)) then we parse new sentences (after training the model on the first 80% sentences). To handle out of vocabulary words we use a combination of [cosine similarity](https://en.wikipedia.org/wiki/Cosine_similarity) and [Damereau Levenshtein distance](https://en.wikipedia.org/wiki/Damerau%E2%80%93Levenshtein_distance). 

N.b.: one must first unzip the file `polyglot-fr.pkl`.

There is 2 ways to run the program either by running the notebook, `TD2 LAPASSAT.ipynb` or with the `run.sh`. In any case one must place the files `sequoia-corpus+fct.txt` and `polyglot-fr.pkl` (for this one just unzip it) at the root of the scripts, notebook (or change the paths in the scripts, notebook). If you are using the notebook, you can just run it to obtain the results. With `run.sh` one can run the program using `chmod u+x run.sh` (couldn't test it since I'm on windows) and then run `./run.sh` (no argument needed, if you still want to test it on other datasets just change the file `sequoia-corpus+fct.txt`, keep the same name, we use the same split 80%-10%-10%).



