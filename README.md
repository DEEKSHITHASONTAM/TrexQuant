# Hangman Game API
================================

## Guess Function Implementation
### 

The core component of this project is the `guess` function, which is responsible for making letter guesses in the game of Hangman. Below is a detailed explanation of its logic:

### TrieNode Data Structure

The TrieNode data structure is utilized to efficiently store and retrieve words for the Hangman game. This approach enables fast lookups and is particularly useful for managing large dictionaries of words.

### Function Logic

The TrieNode tree stores all the words present in the data and retrieves all possible words based on the given input. From these possible words, the function returns the maximum frequency character that occurs. If the character has already been guessed, the function returns the second maximum frequency character from the possible words for the input.

### Memory Efficiency

To ensure memory efficiency, the frequencies of each character are updated every 1000 words, and the possible words are cleared to prevent memory overflow and exceedance of memory limits. This approach enables the function to retrieve possible words through the traverse function in TrieNode and update them efficiently for every input.

### How it Works

#### Step 1: TrieNode Tree Construction

The TrieNode tree is constructed by storing all the words present in the data. This allows for fast lookups and efficient management of large dictionaries of words.

#### Step 2: Possible Words Retrieval

The TrieNode tree retrieves all possible words based on the given input. This is done by traversing the TrieNode tree and finding all words that match the input.

#### Step 3: Maximum Frequency Character Selection

From the possible words, the function returns the maximum frequency character that occurs. If the character has already been guessed, the function returns the second maximum frequency character from the possible words for the input.

#### Step 4: Memory Efficiency Updates

To ensure memory efficiency, the frequencies of each character are updated every 1000 words, and the possible words are cleared to prevent memory overflow and exceedance of memory limits.
