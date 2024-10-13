- Better than stemming
- Slower
- Finds root word
- Ouput is called lemma

## Wordnet Lammatizer

```python
nltk.stem import wordnetLemmatizer
lemmatizer = wordnetLemmatizer()

lemmatizer.lemmatize(word,pos='v')
```
```
Noun      - n
Verb      - v
Adjective - a
Adverb    - r
```
```

