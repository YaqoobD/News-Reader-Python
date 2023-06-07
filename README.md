# News Reader with Python 📰🐍

## Motivation 🌟

To collect dataset of the recent technology news from different resources, and the applying some NLP techniques in order to analyze to most common trend of technology. For Machine Learning task we would do "Topic Modeling". Topic Modeling is an unsupervised learning approach to clustering documents, to discover topics based on their contents. It is very similar to how K-Means algorithm and Expectation-Maximization work. 

## Data Scraping 🕷️📊

The data was acquired from many websites such as: inshort, linux magazine, BBC technology, google news AI canada, yahoo tech and google news computing canada.The data is scrapped as html file, parsed using BeautifulSoup, and then the relevant information is extracted and stored in csv file. Depending on the accessibility of each website, sometimes the urllib is used and sometimes requests, i.e the request using urllib is forbidden in some website.

## NLP Processing 📝🔍
![image](https://user-images.githubusercontent.com/52135942/212906115-8f681992-bd91-4d9b-8ce5-ae29abc4ef2d.png)

## Stop Words ⛔🔡

![image](https://user-images.githubusercontent.com/52135942/212906192-8bb19b0b-843c-451f-95b7-bfe565114e14.png)
![image](https://user-images.githubusercontent.com/52135942/212906243-7934c6b0-2071-410f-bce6-789ae04fe4b7.png)

## Topic Modeling with LDA and NMF 📑🔍F
Topic Modeling is an unsupervised learning approach to clustering documents, to discover topics based on their contents.

### LDA 🔍

LDA, or Latent Derelicht Analysis is a probabilistic model, and to obtain cluster assignments, it uses two probability values: P( word | topics) and P( topics | documents). These values are calculated based on an initial random assignment, after which they are repeated for each word in each document, to decide their topic assignment. In an iterative procedure, these probabilities are calculated multiple times, until the convergence of the algorithm.

### NMF 📑

Non-negative Matrix Factorization is a Linear-algeabreic model, that factors high-dimensional vectors into a low-dimensionality representation. Similar to Principal component analysis (PCA), NMF takes advantage of the fact that the vectors are non-negative. By factoring them into the lower-dimensional form, NMF forces the coefficients to also be non-negative

![image](https://user-images.githubusercontent.com/52135942/212906610-3da1db51-bd1f-4c28-9033-be30e1497679.png)

![image](https://user-images.githubusercontent.com/52135942/212906681-ace6a210-376d-4edc-b24c-807e2c569343.png)

![image](https://user-images.githubusercontent.com/52135942/212906720-8d484c2c-1e80-4432-b413-9eb8dd62c79d.png)

## Conclusion 📝

The two tables above, in each section, show the results from LDA and NMF on both datasets. There is some coherence between the words in each clustering. For example, Topic # 01 in LDA shows words associated with production and platform, as evident with words such as “Intel”, “chip”, “windows”, “Nintendo, and “website”. Other topics show different patterns.

On the other hand, comparing the results of LDA to NMF also shows that NMF performs better. Looking at Topic # 03, we can see there are many Tech devices clustered into the same category, along with the word “patent”. This type of headline is very common in news articles, with wording similar to “galaxy Smartphone with camera” or “vivo”.

We also see two topics related to violence. First, Topic # 04 focuses on bias related terms, such as “find”, “bert”, “sentiment”, “against”, and “privacy”. Second, Topic # 07 focuses on terms, such as “Intelligence”, “responsible”, “lawsuit”, and “voice”. This is an interesting split between the topics because although the terms in each are very closely related, one focuses more on biases, and the other more on Artificial Intelligence. the results show that NMF performs much better than LDA. 🌍📰🔍









