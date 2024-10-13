- words which won't play crucial role in meaning of paragraph
- is,the etc like words
```python

from nltk.corpus import stopwords

import nltk
nltk.download('stopwords')

stopwords.words('english')
```

#### Stemming
```python
from nltk.stem import SnowballStemmer

stemmer = SnowballStemmer()

sentences = nltk.sent_tokenize(corpus)

for i in range(len(sentences)):
	words = nltk.word_tokenize(sentences[i])
	words = [stemmer.stem(word) for word in words if word not in set(stopwords.words('english'))]
	sentences[i] = ' '.join(words)
```

#### Lemmatizing
```python
from nltk.stem import WordnetLemmatizer

lemmatizer = WordnetLemmatizer()

sentences = nltk.sent_tokenize(corpus)

for i in range(len(sentences)):
	
	words = nltk.word_tokenize(sentences[i])
	words = [lemmatizer.lemmatize(word.lower(),pos='v') for word in words if word not in set(stopwords.words('english'))]
	sentences[i] = ' '.join(words)
```