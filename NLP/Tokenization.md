## 1. Corpus->Documents
(Paragraphs -> List of Sentences)

```python
from nltk.tokenize import sent_tokenize

documnets = sent_tokenize(corpus)
```

Splits based on full stops(.) or exclamations(!)

## 2. Corpus->Words
(Paragraphs -> List of Words)

```python
from nltk.tokenize import word_tokenize

words = words_tokenize(corpus)
```

#### Wordpunct Tokenize
```python
from nltk.tokenize import wordpunct_tokenize

words = words_tokenize(corpus)
```

Split words like Bob's -> Bob, ' , s

#### Treebank Word Tokenizer
```python
from nltk.tokenize import treebankWordTokenizer
t = treebankWordTokenizer()
t.tokenize(corpus)
words = words_tokenize(corpus)
```
Wont split full stop except last full stop
splitting => bob. was -> bob. , was