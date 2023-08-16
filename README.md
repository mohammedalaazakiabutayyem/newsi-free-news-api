# Newsi News API

## Overview

Free News API is able to fetch local news and category news in real time.

Please email mohammedalaazakitayyem@gmail.com if you find any bugs.
This api works with :[Newsi](https://newsi-app.com)

## The News api

This news API supports local news and category news.

1. Top Headlines news
2. Local news
3. World news
4. business news
5. sports news
6. world news
7. politics news
8. technology news
9. entertainment news
10. science news








## Supported-language-and-countries

To get the country and its supported language

```
https://newsi-app.com/api/local?language={language_code}&country={country_code}&sort={sort_by}&page={page_count}&limit={news_limit}
```

Example - https://newsi-app.com/api/Supported-language-and-countries

```JSON
  {
    "United States": [
      {
        "Country code": "us",
        "Language code": "en",
        "Language name": "English"
      }
    ]
  },
```

---



## Local news

Make a get request specifying the local of news you want

Field | Description
------|------------
language | The 2-letter ISO-639-1 code of the language you want to get headlines for. example: ```ar``` ```en``` ```es``` ```fr``` ```he``` .....
country | Find sources that display news in a specific country. Possible options: .```eg``` ```us``` ```es``` ```fr``` ```in``` .....
sort | The order to sort the articles in :<br/>```top``` = Fetch the top news.<br/>```last``` = Fetch the latest news.
page | Use this to page through the results.
limit | Use this to customize the number of stories per page <br/>```default``` = 20<br/> ```Max``` = 100

```
https://newsi-app.com/api/local?language={language_code}&country={country_code}&sort={sort_by}&page={page_count}&limit={news_limit}
```

Example - https://newsi-app.com/api/local?language=en&country=us&sort=top&page=1&limit=20

```JSON
  {
    "_id": "7cdb7212a8bdf75e6fe105ac6059e8cf7e8d089a825ae49d70fa309f563af7fb",
    "hasBody": true,
    "image": "https://lh6.googleusercontent.com/proxy/LXN_GTwpp2ymuhK9maK5rx7wZM1owJ105rnAP3eMFqu8_xaTXLFQ7_j-o_WuzlCZxfFukxtMCVF0YOujwMfM4IRy2L4BA00tfqNJaTmfTtICNYMgewnPVToLap0dJfJPzLfP2C_i3Sz6ecpKTjFoyYBvLtYQk6s7HKpxic43lTYdcJMarU47B1bNiAM9YA=s1200",
    "link": "https://www.nytimes.com/2023/08/15/us/elections/trump-indictment-georgia-charges-takeaways.html",
    "publishedAt": "2023-08-16T06:08:30Z",
    "publishedTimestamp": 1692158910,
    "shortLink": "nytimes.com",
    "sourceName": "The New York Times",
    "title": "Key Takeaways from the Trump Indictment in Georgia"
  },
```

---




## Category news

Make a get request specifying the Category of news you want

Field | Description
------|------------
category | The category you want to get new for. Possible options:```sport``` ```world``` ```business``` ```science_and_technology``` ```education``` ```entertainment``` ```health``` ```travel```.
language | The 2-letter ISO-639-1 code of the language you want to get headlines for. example: ```ar``` ```en``` ```es``` ```fr``` ```he``` .....
country | Find sources that display news in a specific country. Possible options: .```eg``` ```us``` ```es``` ```fr``` ```in``` .....
sort | The order to sort the articles in :<br/>```top``` = Fetch the top news.<br/>```last``` = Fetch the latest news.
page | Use this to page through the results.

```
https://newsi-app.com/api/local?category={language_code}&language={language_code}&country={country_code}&sort={sort_by}&page={page_count}
```

Example - https://newsi-app.com/api/local?category=world&language=en&country=us&sort=top&page=1

```JSON
  {
    "_id": "7cdb7212a8bdf75e6fe105ac6059e8cf7e8d089a825ae49d70fa309f563af7fb",
    "hasBody": true,
    "image": "https://lh6.googleusercontent.com/proxy/LXN_GTwpp2ymuhK9maK5rx7wZM1owJ105rnAP3eMFqu8_xaTXLFQ7_j-o_WuzlCZxfFukxtMCVF0YOujwMfM4IRy2L4BA00tfqNJaTmfTtICNYMgewnPVToLap0dJfJPzLfP2C_i3Sz6ecpKTjFoyYBvLtYQk6s7HKpxic43lTYdcJMarU47B1bNiAM9YA=s1200",
    "link": "https://www.nytimes.com/2023/08/15/us/elections/trump-indictment-georgia-charges-takeaways.html",
    "publishedAt": "2023-08-16T06:08:30Z",
    "publishedTimestamp": 1692158910,
    "shortLink": "nytimes.com",
    "sourceName": "The New York Times",
    "title": "Key Takeaways from the Trump Indictment in Georgia"
  },
```

---
