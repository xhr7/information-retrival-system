# information-retrival-system
Information Retrival process: Indexing ,Matching,Resulte.
Create a System to index and search 10 textual documents (.txt files) and I uploaded it to the drive to make it easier to use in Google Colab
First I created 12 document, 10 of them talk about data structures and 2 talk about completely different topics, one about birds and the other about saffron.
then I Index my data using the indexing techniques 

1- Text Indexing techniques:

-Word Exraction

-Tokenization 

-Lower casing

-Stop words removel 

2-Normalization

-Stemming

-Lemmatization

3-Term weighting methods

-TF*IDF

I started use word extraction,First I used the tokenise, I separated all the words in the file and also deleted the punctuation marks and special characters then Stop words removel I have deleted all the words in the stop word in ntlk library ,After that I converted all the text to lowercase ,And the second thing she used was the Lemmatization and stemming are two text normalization techniques that aim to reduce inflected words to their base form (i.e., lemma or root form). While both techniques have their own advantages and disadvantages, using them together can often yield better results than using either technique alone.
Stemming involves removing suffixes from words to obtain their root form. This process is relatively simple and fast, but it can sometimes result in incorrect stems, as some words may have multiple possible stems. For example, the word "running" could be stemmed to "run" or "running", depending on the specific stemming algorithm used.
Lemmatization, on the other hand, involves using a dictionary or morphological analysis to determine the base form of a word. This technique is more accurate than stemming, as it takes into account the context and part of speech of the word. However, it is also more computationally intensive and slower than stemming.
By combining stemming and lemmatization, we can take advantage of the speed and simplicity of stemming while also correcting some of its errors using lemmatization. This can result in better text normalization, which can ultimately improve the performance of downstream natural language processing tasks such as text classification or information retrieval.
then I use TF_IDF for weight for each word , the importent word should haa imprtent wegight

Then we allow the user to enter the query, and we also do an index for it. The last thing we start is to calculate the similarity between the query that the user entered and the files in the drive, and the files closest to the user's query are returned to me in descending order.
