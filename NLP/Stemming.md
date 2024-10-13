- Simplifying words
- Faster
- Find root stem
- Not a efficient method

eating,eaten,eat => eat

## Porter Stemmer

```python
from nltk.stem import PorterStemmer
stemming = PorterStemmer()
for word in words:
	stemming.stem(word)
```

It wont work for some words
History => Histori

## Regexp Stemmer

```python
from nltk.stem import RegexpStemmer
stemming = RegexpStemmer('ing$|s$|e$|able$', min =4)
for word in words:
	stemming.stem(word)
```

$ says only coming in last takes into consideration

## Snowball Stemmer

```python
from nltk.stem import SnowballStemmer
stemming = SnowballStemmer('english')
for word in words:
	stemming.stem(word)
```

Better than normal stemmer
capital letters converted before stemming

	normal   : fairly => fairli
	snowball : fairly=>fair