# Songs of the Self: Using Stylometry to Describe Relations of Literary Influence



## How can computational methods describe the Pessoa-Whitman connection?

This study investigates the literary styles of Fernando Pessoa and his heteronyms, in order to determine to what extent they reflect the strong influence that Walt Whitman is theorized to have had on Pessoa. The research was conducted in two parts, both relying on stylometry. Firstly, a corpus consisting of poems released under Pessoa's orthonymous self and his heteronyms, Alberto Caeiro, Ricardo Reis and Alvaro de Campos were scraped from a compilation of his works. These were then subjected to a cluster analysis using the Stylo package in R, which included a corpus of poems by Walt Whitman, and a distractor corpus of H. P. Lovecraft's and Wilfred Owen's poetry. The purpose of this was to identify how stylistically similar Whitman's Poetry is to Pessoa's in comparison to an arbitrarily selected corpus. Secondly, Pessoa and his heteronyms, (except for Reis, as his corpus contained too few words for this step) were compared in relation to Whitman's works, this was to check for any difference in stylistic similarity between Whitman and the heteronyms. This will hopefully generate a discussion about the effectiveness of using stylometry to examine the relations of influence between authors.

### Data
#### A Little Larger than the Entire Universe
The data consisted of several corpora of poetry. For poems written by Pessoa, the majority of them are scraped from a collection of Pessoa's works by Richard Zenith called ‘A Little Larger Than the Entire Universe’ from [archive.org]([url](https://archive.org/details/fernando-pessoa-a-little-larger-than-the-entire-universe-selected-poems-penguin-classics-2006/Fernando%20Pessoa%20A%20Little%20Larger%20Than%20the%20Entire%20Universe%20Selected%20Poems%20Penguin%20Classics%202006/
) using the PyPDF module for Python. This resulted in 77 poems by Pessoa, 52 by Caeiro, 56 by Reis and 41 by Campos.
##### CSV key
| Index | Formatted_text | Cleaned_text | Tokenized_text | Heteronym |
| ----- | -------------- | ------------ | -------------- | --------- |
| The poem's index within its heteronym's corpus. NOTE: When joining poems which span across multiple pages, the order of the poems within their corpora may have been changed, and thus, might not align with the order in which they are presented in the book. | The poem with all excess whitespace and line breaks removed, but the original punctuation is still included. | The poem with all whitespace, line breaks and punctuation removed. | The tokenized poem with all punctuation and stopwords removed. | The name of the heteronym to whom the poem is attributed. |

#### 35 Sonnets and English Poems vol.1 & 2
Also included in the main corpus are the poems included in Pessoa's "35 Sonnets" collection, and 27 poems from the "English Poems" collection. These poems were sourced from Project Gutenberg as .txt files and cleaned using Python regular expressions.

#### Whitman
The main body of text that we will be comparing the stylistic similarity of Pessoa and his heteronyms too is from Walt Whitman's 'Leaves of Grass' which contains 389 poems. This was a premade dataset provided by Johnmberger https://github.com/johnmberger/walt-whitbot.git.

#### Lovecraft
As a distractor corpus, 48 poems by American author H. P. Lovecraft were selected. These poems were scraped from https://www.hplovecraft.com/writings/texts/ using ScraPy and BeautifulSoup, as part of a previous project, and were thus chosen to be used as a distractor corpus.
##### CSV key
||Title|Text_Original|Text_Continuous|Link|
|---|---|---|---|---|
|Contains the poem/row count.|Contains the title of the poem.|Contains the poem itself, in its original form.|Contains the poem itself, with all indents and line breaks removed.|Contains the hyperlink to the page that the poem was scraped from.|

#### Owen
Finally, the distractor corpus was completed with 25 poems by British author Wilfred Owens. These poems were manually copied from "Poems by Wilfred Owen", provided by Project Gutenberg, also as part of a previous project.

### Structure 
This repository contains various files, these include:
- pessoa.pdf (A PDF edition of "A Little Larger Than the Entire Universe")
- Pessoa_Heteronyms_Scraping.ipynb (Jupyter notebook containing the code for scraping the corpus)
- README.md (ReadMe)
- Stylo.zip (Compressed folder containing the outputs of the stylo analysis, and the joined .txt files that were used in producing them)
- T&M Group Report.pdf (The research report)
- pessoa_heteronyms_full_corpus.csv (The main Pessoa corpus, exported as .csv)
- Caeiro (Directory containing the Caeiro corpus)
- Campos (Directory containing the Campos corpus)
- Distractor_Corpus (Directory containing the entire distractor corpus, csv of the Lovecraft corpus, and jupyter notebook containing the code used to scrape the Lovecraft corpus)
- Pessoa (Directory containing the Pessoa corpus. Including the scraped poems from "A Little Larger than the Entire Universe", 35 Sonnets and English Poems vol. 1&2)
- Reis (Directory containing the Reis corpus)

### How to use
In order to access this repository, you will need software that is able to run Jupyter Notebook (or .ipnyb) files. You will also need to ensure that the following Python modules are installed, in order for the code to run properly:
- re
- pypdf
- pandas
- os
- nltk

Thirdly, it is advised to install R to use the Stylo package for stylometry.

### Intended use of this repository
Pessoa's vast heteronymous corpus has, as of early 2025, been mostly unexplored through digital humanities methods. In this project, we have the datasets of Pessoa, as well as various other authors, freely available for other researchers to use. We also have provided the methods by which we stylometrically analysed these works, and the conclusions we drew, in case any future researchers wish to use this repository, and its findings,  for their own benefit.

### Licenses
Each poet's works used in this project falls under the public domain, and is thus free to be used for our research.

### Collaborators
  This repository was created by Gheorghe Septelici, Henry Hornung and Aidan Grefte.  
  https://github.com/gheorgheseptelici  
  https://github.com/HenryAHornung  
  https://github.com/Aiclan  
