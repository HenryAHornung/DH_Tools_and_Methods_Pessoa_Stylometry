# Songs of the Self: Using Stylometry to Describe Relations of Literary Influence



#### How can computational methods describe the Pessoa-Whitman connection?

This study investigates the literary styles of Ferando Pessoa and his heteronyms, in order to determine to what extent they reflect the strong influence that Walt Whitman is theorized to have had on Pessoa. The research was conducted in two parts, both relying on stylometry. Firstly, a corpus consisting of poems released under Pessoa's orthynomous self and his heteronyms, Alberto Caeiro , Ricardo Reis and Alvaro de Campos were scraped from a compilation of his works. These were then subjected to a cluster analysis using the Stylo package in R, which included a corpus of poems by Walt Whitman, and distractor corpus of H. P. Lovecraft's and Wilfred Owen's poetry. The purpose of this was to identify 

## Data
a corpus consisting of poems released under Pessoa's orthynomous self (77 poems) and his heteronyms, Alberto Caeiro (52 poems), Ricardo Reis (56) and Alvaro de Campos (41 poems)

The corpus this we are using a selection created by Richard Zenith called ‘A Little Larger Than the Entire Universe’ from archive.org. This book contains many poems that had never been translated before, many of them coming from Zenith translating the original manuscript. However, some of the works in this book were never published by Pessoa himself, which may mean he never wanted them to be a part of this heteronyms oeuvre. Regardless, the selection will still serve as a useful database for our research.

https://archive.org/details/fernando-pessoa-a-little-larger-than-the-entire-universe-selected-poems-penguin-classics-2006/Fernando%20Pessoa%20A%20Little%20Larger%20Than%20the%20Entire%20Universe%20Selected%20Poems%20Penguin%20Classics%202006/

## Structure 
This repository contains various files, these include:

### step 1: stylometry with distractors.
- Corpora broken down into six parts.

### step 2: opposing whitman to each of Pessoa's heteronyms.
- Reis removed from selection, since his corpus is too small.
- The first test didn't reveal particularly similar styles between any of the heteronyms and whitman, so we need to take a closer look at how they differ.


### CSV key
| Index | Formatted_text | Cleaned_text | Tokenized_text | Heteronym |
| ----- | -------------- | ------------ | -------------- | --------- |
| The poem's index within its heteronym's corpus. NOTE: When joining poems which span across multiple pages, the order of the poems within their corpora may have been changed, and thus, might not align with the order in which they are presented in the book. | The poem with all excess whitespace and line-breaks removed, but the original puntcuation still included. | The poem with all whitespace, line-breaks and punctuation removed. | The tokenized poem with all punctuation and stopwords removed. | The name of the heteronym to whom the poem is attributed. |

## How to use

## Intended use of this repository

## Licenses
Pessoa's poetry falls under the public domain, and is thus free to be used for our research.

## Collaborators
  This repository was created by Gheorghe Septelici, Henry Hornung and Aidan Grefte.  
  https://github.com/gheorgheseptelici  
  https://github.com/HenryAHornung  
  https://github.com/Aiclan  
