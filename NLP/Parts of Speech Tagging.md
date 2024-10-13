```python
nltk.download('averaged_perceptron_tagger')
words = nltk.word_tokenize(sentence)
pt = nltk.pos_tag(words) #list of words input

pts = nltk.pos_tag_sents("Taj Mahal is Beautiful") #then each letter is taken
nltk.pos_tag("Taj Mahal is Beautiful".split())
```

| **Tag**  | **Description**                          | **Example**         |
| -------- | ---------------------------------------- | ------------------- |
| **CC**   | Coordinating conjunction                 | and, but, or        |
| **CD**   | Cardinal number                          | one, two, 100       |
| **DT**   | Determiner                               | the, a, an          |
| **EX**   | Existential there                        | there is, there was |
| **FW**   | Foreign word                             | bonjour, gracias    |
| **IN**   | Preposition or subordinating conjunction | in, on, because     |
| **JJ**   | Adjective                                | blue, fast, tall    |
| **JJR**  | Adjective, comparative                   | better, faster      |
| **JJS**  | Adjective, superlative                   | best, fastest       |
| **LS**   | List item marker                         | 1., 2., A., B.      |
| **MD**   | Modal                                    | can, will, might    |
| **NN**   | Noun, singular or mass                   | cat, car, water     |
| **NNS**  | Noun, plural                             | cats, cars          |
| **NNP**  | Proper noun, singular                    | John, London        |
| **NNPS** | Proper noun, plural                      | Smiths, Americas    |
| **PDT**  | Predeterminer                            | all, both, half     |
| **POS**  | Possessive ending                        | John's, cat's       |
| **PRP**  | Personal pronoun                         | I, you, he          |
| **PRP$** | Possessive pronoun                       | my, your, his       |
| **RB**   | Adverb                                   | quickly, never      |
| **RBR**  | Adverb, comparative                      | faster, better      |
| **RBS**  | Adverb, superlative                      | fastest, best       |
| **RP**   | Particle                                 | up, off, down       |
| **SYM**  | Symbol                                   | $, %, &             |
| **TO**   | to                                       | to go, to play      |
| **UH**   | Interjection                             | oh, wow, ouch       |
| **VB**   | Verb, base form                          | eat, run, jump      |
| **VBD**  | Verb, past tense                         | ate, ran, jumped    |
| **VBG**  | Verb, gerund or present participle       | eating, running     |
| **VBN**  | Verb, past participle                    | eaten, driven       |
| **VBP**  | Verb, non-3rd person singular present    | eat, run            |
| **VBZ**  | Verb, 3rd person singular present        | eats, runs          |
| **WDT**  | Wh-determiner                            | which, that         |
| **WP**   | Wh-pronoun                               | who, what           |
| **WP$**  | Possessive wh-pronoun                    | whose               |
| **WRB**  | Wh-adverb                                | when, where, why    |

