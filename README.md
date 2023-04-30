# Fine-tuning-GPT-3-for-Poetry-Generation-and-Evaluation

version: 2023.04.28

author: PeterS

This repository contains the datasets and code for the paper "On the power of special-purpose GPT models to create and evaluate new poetry in old styles" by Piotr Sawicki, Marek Grześ, Fabricio Goes, Dan Brown, Max Peeperkorn, Aisha Khatun, Simona Paraskevopoulou
due to be published in ICCC'23 Proceedings.

link: https://github.com/PeterS111/Fine-tuning-GPT-3-for-Poetry-Generation-and-Evaluation/blob/main/sawicki2023gptpoetry.pdf

All poems in the Datasets are out of copyrights, and have been scraped from https://gutenberg.org/ and https://www.poetryfoundation.org/ .

  Poets included in the Datasets are:

  * Ella Wheeler Wilcox, 1850–1919, United States

   * Rudyard Kipling, 1865–1936, England

   * Emily Dickinson, 1830–1886, United States 

   * Lord Byron, 1788–1824, England/Italy

   * William Wordsworth, 1770–1850, England

   * Walt Whitman, 1819–1892, United States 

   * Thomas Hardy, 1840–1928, England


Datasets include only the poems of the above authors that are between 100 and 500 words in length.

Datasets include:

1. Collection of poems without summaries and themes, with separate folders for each author, with a detailed list of these poems (number of poems per author varies).
2. Collection of poems with GPT-3.5 -generated summaries and themes for each poem, with separate folders for each author (300 poems per author), with a detailed list of these poems.
3. Combined collection of poems with GPT-3.5 -generated summaries and themes of all seven authors (300 poems per author)
4. .jsonl files for each separate author (7 files) and combined .jsonl file of all authors. These files are ready to be used for fine-tuning GPT-3.
5. Additional authors:

* William Ernest Henley, 1849–1903, England

* Christina Rossetti, 1830–1894, England

Datasets for both additional authors include 150 poems with summaries and themes for each author, with a detailed list of poems for each author.

For detailed explanation of the dataset please refer to the paper mentioned above. 


Code includes: 

1. Notebook for preparing .jsonl files (to be used for GPT-3 fine-tuning) from our datasets
2. Notebook for fine-tuning GPT-3
3. Notebook for generating poetry from the fine-tuned models
