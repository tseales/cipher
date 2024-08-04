# cipher
## Goal
The goal of this project was to take a text file as input and decipher the hidden code. Each line of the cipher is in a 'number:word' key format. When the numbers are sorted into a pyramid structure - with each line of the pyramid being comprised of the total instance of numbers 1 greater than the line before it - the last number's word pairing returns a word to be used in the final cipher. *See image below:*

![pyramid-ex](https://github.com/user-attachments/assets/b1e8f544-9441-4ea7-9adb-77957fa93688)

The 'decode' function expects the text file as an input, separates the number:word pairings into a Pandas DataFrame which is then sorted (ascending) to maintain the integrity of pairings. Once sorted, a *for* loop is utilized to create the pyramid structure used to map the last number in each line of the pyramid to its associated word-pairing housed in the aforementioned Pandas DataFrame. When each text to be used in the final cipher is found, it is stored until all text has been gathered for a final output.

An example text file is included in the repo.
