# Exploring Pessoa’s Heteronymous Biographies Through a Computational Approach

<a title="Template:Cavalão, Public domain, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Pessoa_chapeu.jpg"><img width="256" alt="Fernando Pessoa, 1914" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/32/Pessoa_chapeu.jpg/256px-Pessoa_chapeu.jpg?20170303141045"></a>

#### How efficient are sentiment, type-token ratio and word-frequency analyses in elucidating the stylistic peculiarities of Pessoa and his heteronyms' poems?

This project aims to identify the link between Fernando Pessoa’s heteronymous identities and their manufactured biographies. Over the course of his life Pessoa expanded the story of each of his Heteronyms, namely Ricardo Reis, Alvaro De Campos and Alberto Caeiro. We want to use stylistic techniques such as sentiment analysis and word frequency analysis and type-token ratio analysis to discover if Fernando Pessoa was able to accurately portray his heteronyms' biographies in their poetry. For this we are using a selection created by Richard Zenith called ‘A Little Larger Than the Entire Universe’ from archive.org. This book contains many poems that had never been translated before, many of them coming from Zenith translating the original manuscript. However, some of the works in this book were never published by Pessoa himself, which may mean he never wanted them to be a part of this heteronyms oeuvre. Regardless, the selection will still serve as a useful database for our research.

https://archive.org/details/fernando-pessoa-a-little-larger-than-the-entire-universe-selected-poems-penguin-classics-2006/Fernando%20Pessoa%20A%20Little%20Larger%20Than%20the%20Entire%20Universe%20Selected%20Poems%20Penguin%20Classics%202006/

## Structure 
This repository contains various files, these include:
- pessoa.pdf (A PDF edition of "A Little Larger Than the Entire Universe")
- "file" (Jupyter notebook containing the code for scraping and analysing the corpus)
- "caeiro" (Directory containing .txt files of each poem in the Caeiro sub-corpus)
- "reis" (Directory containing .txt files of each poem in the Reis sub-corpus)
- "campos" (Directory containing .txt files of each poem in the Campos sub-corpus)
- "pessoa" (Directory containing .txt files of each poem in the Pessoa sub-corpus)
- pessoa_heteronyms_full_corpus.csv (A CSV file containing the entire scraped corpus)

### CSV key
| Index | Formatted_text | Cleaned_text | Tokenized_text | Heteronym |
| ----- | -------------- | ------------ | -------------- | --------- |
| The poem's index within its heteronym's corpus. NOTE: When joining poems which span across multiple pages, the order of the poems within their corpora may have been changed, and thus, might not align with the order in which they are presented in the book. | The poem with all excess whitespace and line-breaks removed, but the original puntcuation still included. | The poem with all whitespace, line-breaks and punctuation removed. | The tokenized poem with all punctuation and stopwords removed. | The name of the heteronym to whom the poem is attributed. |

## How to use
In order to access this repository, you will need software that is able to run Jupyter Notebook (or .ipnyb) files. You will also need to ensure that the following python modules are installed, in order for the code to run properly:
- re
- pypdf
- pandas
- os
- nltk
- collections
- matplotlib.pyplot
- seaborn

While the entire corpus will be accessible through the jupyter notebook, it is also provided in the repository as a csv file, and multiple txt files, so being able to open these file types may be helpful when accessing the data.
NOTE: In order for the active learning exercise to work, it is advised to keep the structure of the directory as it is in the GitHub repository.

## Intended use of this repository
Pessoa's vast heteronymous corpus has, as of early 2025, been mostly unexplored through digital humanities methods. In this project, we assembled a corpus and subjected it to three initial computational analyses. However, this only entails a preliminary investigation, and we invite researchers to use our corpus to further study Pessoa's works. Moreover, our research contains an evaluation of sentiment analysis, type-token ratio and word frequency for thematic analyses, specifically pertaining to poetry.

## Licenses
Pessoa's poetry falls under the public domain, and is thus free to be used for our research.

## Collaborators
  This repository was created by Gheorghe Septelici, Henry Hornung and Aidan Grefte.  
  https://github.com/gheorgheseptelici  
  https://github.com/HenryAHornung  
  https://github.com/Aiclan  
