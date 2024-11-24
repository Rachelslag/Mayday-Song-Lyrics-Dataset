# Mayday Song Lyrics Dataset

This dataset contains song lyrics of a few songs by the Taiwanese rock band Mayday. Mayday’s popularity extends beyond Taiwan and has spread across the Sinophone world, including mainland China, Hong Kong, Singapore, and more.

Using this dataset, researchers can study Mayday’s lyrical themes and linguistic style. Additionally, the dataset can be useful for scholars doing cultural analysis, as Mayday’s songs are known to capture the zeitgeist of Taiwanese youth in the mid to late 1990s. Furthermore, they are sometimes referred to as the 'Beatles of Asia'. Comparative analysis could be performed to examine if the songs have similar topics or styles.

The song lyrics of the selected tracks have been extracted from the website [genius.com](https://genius.com). Since Genius only provides lyrics for a limited number of songs, the top five songs have been selected for inclusion in this dataset.

The text files containing the lyrics have been placed into a `corpus` folder and preprocessed using the Chinese language model of spaCy. Tokenization, lemmatization, and part-of-speech tagging have been applied to all the text files. The enriched dataset has been extracted into a CSV file.

## Column Description

This dataset contains information about song lyrics by Mayday, processed using spaCy. Below is an explanation of each column in the CSV file:

| **Column Name** | **Description**                                                                               |
|------------------|-----------------------------------------------------------------------------------------------|
| `Filename`      | Contains the title of the song in Chinese and English.                                        |
| `Title`         | Contains the title of the song in Chinese and English. |
| `Text`          | Contains the full lyrics of the song.                                                         |
| `Doc`           | Contains the processed spaCy `Doc` objects.                                                   |
| `Tokens`        | Contains the tokenized lyrics.                                                               |
| `Lemmas`        | Currently an empty column because lemmatization does not work on Chinese text.                |
| `POS`           | Contains parts of speech for all tokens in the lyrics.                                        |

**Note**: The `Lemmas` column is included in the file because it is required for this exercise, but it is empty due to the grammatical structure of the Chinese language. In Chinese, words (characters or compounds) do not change form based on grammatical roles (e.g., singular/plural, tense).

