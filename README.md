# Songs of the Self: Using Stylometry to Describe Relations of Literary Influence



#### How can computational methods describe the Pessoa-Whitman connection?

This study investigates the literary styles of Ferando Pessoa and his heteronyms, in order to determine to what extent they reflect the strong influence that Walt Whitman is theorized to have had on Pessoa. The research was conducted in two parts, both relying on stylometry. Firstly, a corpus consisting of poems released under Pessoa's orthynomous self and his heteronyms, Alberto Caeiro , Ricardo Reis and Alvaro de Campos were scraped from a compilation of his works. These were then subjected to a cluster analysis using the Stylo package in R, which included a corpus of poems by Walt Whitman, and distractor corpus of H. P. Lovecraft's and Wilfred Owen's poetry. The purpose of this was to identify how stylistically similar Whitan's Poetry is to Pessoa's in comparison to an arbitrarily selected corpus. Secondly, each heteronym, (except for Reis, as his corpus contained too few words for this step) was individually compared to Whitman's corpus using Stylo's oppose function. The heteronyms/orthonym were compared to each other, with Whitman's corpus being used as a test set to find overlap between the words being used by each corpus.

## Data
### A Little Larger than the Entire Universe
The data consisted of several corpora of poetry. For poems written by Pessoa, the majority of them are scraped from a collection of Pessoa's works by Richard Zenith called ‘A Little Larger Than the Entire Universe’ from [archive.org]([url](https://archive.org/details/fernando-pessoa-a-little-larger-than-the-entire-universe-selected-poems-penguin-classics-2006/Fernando%20Pessoa%20A%20Little%20Larger%20Than%20the%20Entire%20Universe%20Selected%20Poems%20Penguin%20Classics%202006/
) using the PyPDF module for python. This resulted in 77 poems by Pessoa, 52 by Caeiro, 56 by Reis and 41 by Campos.
#### CSV key
| Index | Formatted_text | Cleaned_text | Tokenized_text | Heteronym |
| ----- | -------------- | ------------ | -------------- | --------- |
| The poem's index within its heteronym's corpus. NOTE: When joining poems which span across multiple pages, the order of the poems within their corpora may have been changed, and thus, might not align with the order in which they are presented in the book. | The poem with all excess whitespace and line-breaks removed, but the original puntcuation still included. | The poem with all whitespace, line-breaks and punctuation removed. | The tokenized poem with all punctuation and stopwords removed. | The name of the heteronym to whom the poem is attributed. |

### 35 Sonnets and English Poems vol.1 & 2
Also included in the main corpus are the poems included in Pessoa's "35 Sonnets" collection, and 27 poems from the "English Poems" collection. These poems were sourced from Project Gutenberg as .txt files, and cleaned using python regular expressions.

### Whitman
W

### Lovecraft
As a distractor corpus, 48 poems by American author H. P. Lovecraft were selected. These poems were scraped from https://www.hplovecraft.com/writings/texts/ using ScraPy and BeautifulSoup, as part of a previous project, and were thus chosen to be used as a distractor corpus.

### Owens
Finally, the distractor corpus was completed with 25 poems by British author Wilfred Owens. These poems were manually copied from "Poems by Wilfred Owen", provided by Project Gutenberg, also as part of a previous project.

## Structure 
This repository contains various files, these include:
- 

## How to use
In order to access this repository, you will need software that is able to run Jupyter Notebook (or .ipnyb) files. You will also need to ensure that the following python modules are installed, in order for the code to run properly:
- re
- pypdf
- pandas
- os
- nltk

Thirdly, it is advised to install R to use the Stylo package for stylometry.

## Intended use of this repository

## Licenses
Each poet's works used in this project falls under the public domain, and is thus free to be used for our research.

## Collaborators
  This repository was created by Gheorghe Septelici, Henry Hornung and Aidan Grefte.  
  https://github.com/gheorgheseptelici  
  https://github.com/HenryAHornung  
  https://github.com/Aiclan  
