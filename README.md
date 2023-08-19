# worldnews 

## Installation 
To install, run the following command:
```bash
pip install worldnews
```
## Available agencies

```properties

Brazilian agencies: uol, g1, estadao, r7, 
                    veja, cartacapital, cnnbrasil,
                    terra, ig, olhardigital, 
                    exame, ge

US agencies: skynews, cnn, nbc, 
             cbs, abc, nyt, 
             wp, foxnews, wsj

UK agencies: bbc, theguardian, reuters, euronews

```
## Retrieve news from single agency

To perform a simple news search use the following syntax.
```python
from worldnews import worldNews

agency = "Some agency..."
search_term = "some word"
number_of_results = 10

news = worldNews()
news.set_agency(agency)
news.display_news(number_of_results)
```
## Single search usage

```python
from worldnews import worldNews

agency = "Some agency..."
search_term = "some word"
news = worldNews()
news.set_agency(agency)
news.search_news(search_term)
```
## Search multiple agencies
To perform a search using multiple agencies use:

```python
from worldnews import worldNews

agency1 = 'some agency'
agency2 = 'some agency'
agency3 = 'some agency'
search_term = "some word"

news = worldNews()
news.set_agencies(agency1, agency2, agency3)
news.search_news_agencies(search_term)
```


