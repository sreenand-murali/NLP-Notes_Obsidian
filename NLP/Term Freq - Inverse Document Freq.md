
### Term Frequency (TF)

$$
\text{TF} = \frac{\text{Number of occurrences of the word in the sentence}}{\text{Total number of words in the sentence}}
$$

### Inverse Document Frequency (IDF)

$$
\text{IDF} = \log_e \left( \frac{\text{Total number of sentences}}{\text{Number of sentences containing the word}} \right)
$$



## Sentences
- **s1**: "good girl"
- **s2**: "good boy"
- **s3**: "boy girl good"

## Term Frequency (TF)

| Word  | TF in s1  | TF in s2  | TF in s3  |
|-------|-----------|-----------|-----------|
| good  | 1/2       | 1/2       | 1/3       |
| girl  | 1/2       | 0         | 1/3       |
| boy   | 0         | 1/2       | 1/3       |

## Inverse Document Frequency (IDF)

- **For "good":**
  $$
  \text{IDF} = \log_e \left( \frac{3}{3} \right) = 0
  $$

- **For "girl":**
  $$
  \text{IDF} = \log_e \left( \frac{3}{2} \right)
  $$

- **For "boy":**
  $$
  \text{IDF} = \log_e \left( \frac{3}{2} \right)
  $$



## TF-IDF Values

| Word  | TF-IDF in s1                   | TF-IDF in s2                   | TF-IDF in s3                   |
|-------|--------------------------------|--------------------------------|--------------------------------|
| good  | 0                              | 0                              | 0                              |
| girl  | 1/2 * log(3/2)                | 0                              | 1/3 * log(3/2)                |
| boy   | 0                              | 1/2 * log(3/2)                | 1/3 * log(3/2)                |


## Advantages
- Easy to implement in python
- Fixed Size I/P
- Word Importance is being captured
	- more repeated word in sentences have less imp(good for example)
## Disadvantages
- Sparse Matrix -> Over Fitting
- Still out of vocabulary
	- cant represent new words in vector