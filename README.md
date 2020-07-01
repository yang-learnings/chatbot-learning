# chatbot-learning

With Python

## Natural Language Processing

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

text = "Hello world"
```
