## One-Hot Encoding Example

## Documents:
- **d1**: The food is good
- **d2**: The food is bad
- **d3**: Pizza is amazing

## Vocabulary:

| Word    | Index |
|---------|-------|
| the     | 0     |
| food    | 1     |
| is      | 2     |
| good    | 3     |
| bad     | 4     |
| pizza   | 5     |
| amazing | 6     |

```json
{
  "d1": [
    [1, 0, 0, 0, 0, 0, 0],  // "the"
    [0, 1, 0, 0, 0, 0, 0],  // "food"
    [0, 0, 1, 0, 0, 0, 0],  // "is"
    [0, 0, 0, 1, 0, 0, 0]   // "good"
  ],
  "d2": [
    [1, 0, 0, 0, 0, 0, 0],  // "the"
    [0, 1, 0, 0, 0, 0, 0],  // "food"
    [0, 0, 1, 0, 0, 0, 0],  // "is"
    [0, 0, 0, 0, 1, 0, 0]   // "bad"
  ],
  "d3": [
    [0, 0, 1, 0, 0, 0, 0],  // "is"
    [0, 0, 0, 0, 0, 1, 0],  // "pizza"
    [0, 0, 0, 0, 0, 0, 1]   // "amazing"
  ]
}

```

## Advantages
- Easy to implement in python
## Disadvantages
- Sparse Matrix -> Over Fitting
- For ML algorithm we need Fixed size I/P 
	-  Here matrix size changes with length of words
	- ( d2 : 4 x 7, d3 : 3 x 7 )
- No semantic meaning is captured
	- like cosine diff of word vectors to find similarity
- Out of vocabulary
	- cant represent new words in vector