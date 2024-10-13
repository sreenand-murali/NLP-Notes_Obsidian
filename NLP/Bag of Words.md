
## Documents
- **d1**: The food is good
- **d2**: The food is good
- **d3**: Pizza is amazing
- d4: Food is good good

## Preprocessing Steps
1. **Lowercasing**
2. **Stop Word Removal**

## Vocabulary

| Word    | Index |
|---------|-------|
| food    | 0     |
| good    | 1     |
| bad     | 2     |
| pizza   | 3     |
| amazing | 4     |

## Bag of Words Representation

```json
{
  "d1": [
    [1, 1, 0, 0, 0]   // "food", "good"
  ],
  "d2": [
    [1, 0, 1, 0, 0]   // "food", "bad"
  ],
  "d3": [
    [0, 0, 0, 1, 1]   // "pizza", "amazing"
  ],
  "d4": [
    [1, 2, 0, 0, 0]   // "food", "good" "good" 
  ],
  
}
```

> [!note] **Note**
> In the Binary Bag of Words model, in d4 2 is replaced with 1.

## Advantages
- Easy to implement in python
- Fixed Size I/P
## Disadvantages
- Sparse Matrix -> Over Fitting
- Ordering of the words are changed
- Still no semantic meaning is captured
	- like cosine diff of word vectors to find similarity
- Still out of vocabulary
	- cant represent new words in vector