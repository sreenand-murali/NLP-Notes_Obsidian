```python
nltk.download('averaged_perceptron_tagger')
nltk.download('maxent_ne_chunker')
nltk.download('words')

words = nltk.word_tokenize(sentence)
tag = nltk.pos_tag(words) #list of words input

tag = nltk.pos_tag_sents("Taj Mahal is Beautiful") #then each letter is taken
nltk.pos_tag("Taj Mahal is Beautiful".split())


nltk.ne_chunk(tag).draw()
```