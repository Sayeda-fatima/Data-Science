## Objective
The objective of this assignment is to extract textual data articles from the given URL and perform text analysis to compute variables that are explained below. 

## Data Extraction
Input.xlsx
For each of the articles, given in the input.xlsx file, extract the article text and save the extracted article in a text file with URL_ID as its file name.
While extracting text, please make sure your program extracts only the article title and the article text. It should not extract the website header, footer, or anything other than the article text. 
 

## Data Analysis
For each of the extracted texts from the article, perform textual analysis and compute the following variables.


### Variables
- **Positive Score:** This score is calculated by assigning the value of +1 for each word if found in the Positive Dictionary and then adding up all the values.
- **Negative Score:** This score is calculated by assigning the value of -1 for each word if found in the Negative Dictionary and then adding up all the values. We multiply the score with -1 so that the score is a positive number.
- **Polarity Score:** This is the score that determines if a given text is positive or negative in nature. It is calculated by using the formula: 
- **Polarity Score** = (Positive Score – Negative Score)/ ((Positive Score + Negative Score) + 0.000001).
Range is from -1 to +1
- **Subjectivity Score:** This is the score that determines if a given text is objective or subjective. It is calculated by using the formula: 
- **Subjectivity Score** = (Positive Score + Negative Score)/ ((Total Words after cleaning) + 0.000001).
Range is from 0 to +1
- **Average Sentence Length** = the number of words / the number of sentences
- **Percentage of Complex words** = the number of complex words / the number of words 
- **Fog Index** = 0.4 * (Average Sentence Length + Percentage of Complex words)
- **Average Number of Words Per Sentence** = the total number of words / the total number of sentences
- **Complex words** = Complex words are words in the text that contain more than two syllables
- **Syllable per word** = We count the number of Syllables in each word of the text by counting the vowels present in each word. We also handle some exceptions like words ending with "es","ed" by not counting them as a syllable.
