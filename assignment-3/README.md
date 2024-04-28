# Assignment 3 - Russian Nested Named Entities

## Author
- Fullname: **Andrei Markov**
- Email: **a.markov@innopolis.university**
- Nickname in CodaLab: **markovav**
- GitHub repository: **https://github.com/markovav-official/nlp-assignments/tree/main/assignment-3**

## Solutions description

### Solution 1 (baseline)

**Test F1 score: 0.06**

This solution is a simple baseline that uses knowledge base of named entities to extract named entities from the text. 

The solution is based on the following steps:
1. Save all named entities from the train dataset to a dictionary (word -> label).
2. For each sentence in the test dataset, extract named entities using the dictionary.
3. Calculate F1 score.

### Solution 2 (best solution)

**Test F1 score: 0.65**

This solution using spaCy library trained from scratch on the train dataset. 

The solution is based on the following steps:
1. Convert the train dataset to the spaCy format.
2. Train the spaCy model on the train dataset.
3. For each sentence in the test dataset, extract named entities using the spaCy model.
4. Calculate F1 score.