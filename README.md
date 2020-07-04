# chatbot-learning

With Python

### Natural Language Processing

For natural language processing, we need to start with some text processing.

* Noise Removal - removing any formatting, for example html labels
* Tokenization - separating text into individual words
* Normalization - cleaning text data
   * Stemming - Chopping off prefixes and suffixes
   * Lemmatization - Bring words down to their root word
```python
# regex for removing punctuation!
import re
# nltk preprocessing magic
import nltk
from nltk.tokenize import word_tokenize
from nltk.stem import PorterStemmer
from nltk.stem import WordNetLemmatizer
# grabbing a part of speech function:
from part_of_speech import get_part_of_speech
```

### Parsing Text

Parsing text helps understand the relationship between words.

* **Part of Speech tagging** Identifies parts of speech (NLTK)
* **Named Entity Recognition** Helps identify proper nouns (NTLK)
* **Dependency Grammar** Helps build relationship between words (spaCy)
* **Regex Parsing** Finds certain structures, e.g emails

## Language Models

### Bag of Words Approach
A simple model to use which basically count the times each word has been used.

### N-Gram model
N-Gram model is similar to bag of words but instead we are grouping a bunch of adjacent words and counting them

### Topic Modelling
Group topics together


1. **term frequency-inverse document frequency (tf-idf)**, prioritising less frequent words together
genism, sklearn are python libraries.

2. **latent Dirichlet allocation** statistical model which determines the most commonly used words which keeps poping up in the same context
