# sotu_text_mining
Jupyter Julia notebook to perform text mining on State of the Union addresses by Trump and Obama

State of the Union speech transcripts taken from https://www.presidency.ucsb.edu/documents/presidential-documents-archive-guidebook/annual-messages-congress-the-state-the-union

Made functions to do basic tokenization, find lines containing certain words, get word counts over a text file, and create a set of unique words used.

First, did analysis of the word "hope" to see how often it was used and what context it was used in. Then found counts of the words "war", "very", and "big" weighted by number of speeches given.
Second, made word sets of both Obama's and Trump's speechs and then found the words unique to only one of them with the idea of finding which words were most unique to Obama or Trump. These sets were then used to identify the sentences from any State of the Union that had the highest number of words unique to that president, with the goal of finding the sentences that were most "Obama-esque" or "Trumpian".

Possible improvements would include improved tokenization and text simplification to allow for similar words to be counted together. Removing proper names from the unique word sets would also do a better job of reflecting each president's utilized vocabulary, rather than identifying sentences that referred to guests to the speech (as those were more likely to be flagged unique due to people's names).
