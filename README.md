# Relevant and First Sentences Extraction

## Purpose:
This repository contains a Python script that utilizes web scraping techniques and sentence embeddings to extract relevant sentences from a web page.
The main functionalities include:
1. Extracting relevant sentences from a web page.
2. Extracting the first sentence of an article.
3. Extracting text from specified HTML elements, such as paragraphs.
4. Utilizing NLTK for sentence tokenization.
  
## Libraries/Modules Used:
- [Requests](https://docs.python-requests.org/en/latest/): For sending HTTP GET requests.
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/): For parsing HTML content.
- [NLTK](https://www.nltk.org/): For natural language processing tasks.
- [Sentence-Transformers](https://www.sbert.net/): For sentence embeddings.

## Workflow:
1. Get the URL from the user.
2. Sends an HTTP GET request to a specified URL.
3. Parses the web page content with BeautifulSoup.
4. Extracts relevant content from specified HTML elements, such as paragraphs.
5. Tokenizes the article into sentences using NLTK.
6. Loads the SentenceTransformer model for sentence embeddings.
7. Encodes sentences into vectors using the model.
8. Computes similarity scores between sentences and a reference sentence.
9. Selects sentences above a specified similarity threshold.
10. Provides functions to extract relevant sentences and the first sentence of an article.

## Working Example:
Running the script with the provided URL would yield relevant sentences, as mentioned below:'https://www.theguardian.com/technology/2023/apr/27/elon-musks-statements-could-be-deepfakes-tesla-defence-lawyers-tell-court' would yield 'The lawsuit is scheduled to go into trial on 31 July, adding to growing legal and regulatory scrutiny over Tesla’s Autopilot system' as the only or one of the relevant sentences.

First sentence of the article:Judge in Autopilot death case says defence argument ‘deeply troubling’ and wants Tesla CEO interviewed under oath on safety claims. 

## Key Results:
- Extracts first sentence from article.
- Extracts relevant sentences based on the user defined threshold which determines the number of sentences.

