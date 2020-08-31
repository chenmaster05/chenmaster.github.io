# nhentai API docs

This is not an official documentation, but I figured it out and though other people might want to use it. This will also be a guide for how to use an API for complete beginners.

# Getting the data

To get the data from the API, you need to use the correct links.
The main link to use is obviously:

    https://nhentai.net

or

```
https://t.nhentai.net
```

for thumbnails (marked with `*` below)

or

```
https://i.nhentai.net
```

for images for actual pages (marked with `**` below).

This will be different for other APIs. Don't try to get NASA info from a hentai site.

Here is a cheat-sheet for all of the links you can use to get data (I'll get on to what the stuff wrapped in brackets means):

### Search for comics

    /api/galleries/search?query={QUERY}&page={PAGE=1}&sort={SORT=recent}

### Search for related comics

    /api/gallery/{BOOK_ID}/related

### Search for tag

    /api/galleries/tagged?tag_id={TAG_ID}&page={PAGE=1}&sort={SORT=recent}

### Get details of a certain book

    /api/gallery/{BOOK_ID}

### Get page of book

    **/galleries/{MEDIA_ID}/{PAGE}.{TYPE}

### Get thumbnail of book

    */galleries/{MEDIA_ID}/{PAGE}t.{TYPE}

### Get the cover of the book

    */galleries/{MEDIA_ID}/cover.{TYPE}

The IDs define what book the API should give you. If you are an avid user of the [r/animemes](https://www.reddit.com/r/animemes) You will recognise what a {BOOK_ID} is. (Ahem, 177013 is a good example). 

This is completely separate from a {MEDIA_ID}. The {MEDIA_ID} is used to get the images associated with the book. Above, you can see that it is only used to get the page, thumbnail and cover images.

The {TAG_ID} is just a {BOOK_ID} but only for tags. Cool? Cool.

{PAGE} is the page number of results you want to show, it is defaulted to 1.

{SORT} is the sorting of the books the API returns, this defaults to recent but you also have the choices of:

- popular: return the books in popularity order of all time.
- popular-week, return the books in popularity order of the week.
- popular-today, return the books in popularity order of the current day.

{TYPE} is the file extension of the image, it usually corresponds to one of the following:

- j: jpg
- p: png
- g: gif

# Traversing the JSON

Scary! JSON looks really complicated to a beginner. This section will teach you how to look through the JSON to find the info you need.

So I use the link:

    https://nhentai.net/api/galleries/search?query=female

I will parse this one and only example for reference. 

```js
{
  "result": [
    {
      "id": 256228,
      "media_id": "1331007",
      "title": {
        "english": "[numa] Kiss wa \u00a5300",
        "japanese": "[numa] \u30ad\u30b9\u306f\u00a5300",
        "pretty": "Kiss wa \u00a5300"
      },
      "images": {
        "pages": [
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          },
          {
            "t": "j",
            "w": 1200,
            "h": 1600
          }
        ],
        "cover": {
          "t": "j",
          "w": 350,
          "h": 467
        },
        "thumbnail": {
          "t": "j",
          "w": 250,
          "h": 333
        }
      },
      "scanlator": "",
      "upload_date": 1545159725,
      "tags": [
        {
          "id": 6346, //<- THIS IS A TAG ID
          "type": "language",
          "name": "japanese",
          "url": "/language/japanese/",
          "count": 164713
        },
        {
          "id": 7752,
          "type": "tag",
          "name": "schoolboy uniform",
          "url": "/tag/schoolboy-uniform/",
          "count": 10329
        },
        {
          "id": 7970,
          "type": "artist",
          "name": "numa",
          "url": "/artist/numa/",
          "count": 16
        },
        {
          "id": 10314,
          "type": "tag",
          "name": "schoolgirl uniform",
          "url": "/tag/schoolgirl-uniform/",
          "count": 47892
        },
        {
          "id": 12695,
          "type": "tag",
          "name": "prostitution",
          "url": "/tag/prostitution/",
          "count": 4240
        },
        {
          "id": 33172,
          "type": "category",
          "name": "doujinshi",
          "url": "/category/doujinshi/",
          "count": 185969
        },
        {
          "id": 35762,
          "type": "tag",
          "name": "sole female",
          "url": "/tag/sole-female/",
          "count": 43471
        },
        {
          "id": 35763,
          "type": "tag",
          "name": "sole male",
          "url": "/tag/sole-male/",
          "count": 38831
        }, 
     }
     ..., 
     {...}
  ]
}
```

- result (list)

  - result[0] (dict)

    - id (int): BOOK_ID of the book

    - media_id (int): MEDIA_ID of the book

    - scanlator (str): scanlator of the book

    - upload_date (int): upload date of the book (format unknown)

    - title (dict)

      - english (str): the english title of the book

      - japanese (str): the japanese title of the book

      - pretty (str): the english title of the book without author, parody name and excess information

    - images (dict)

      - cover (dict)
        - t (char): the first character of the extension of the cover
        - w (int): the width of the cover
        - h (int): the height of the cover
      - thumbnail (dict)
        - t (char): the first character of the extension of the thumbnail
        - w (int): the width of the cover
        - h (int): the height of the cover
      - pages (list) (the metadata of the pages IN ORDER)
        - pages[0] (dict)
          - t (char): the first character of the extension of the page
          - w (int): the width of the page
          - h (int): the height of the page
        - pages[1] (dict)
          - same as pages[0]
        - ... continues to pages[num_pages - 1]

    - tags (list)

      - tags[0] (dict)
        - id (int): TAG_ID of the tag
        - type (str): the type of the tag (whether its a language tag or a parody tag or just a tag)
        - name (str): the name of the tag
        - url (str): the relative url of the tag stored in nHentai's server
        - count (int): the number of books with the tag
      - tags[1] (dict)
        - same as tags[0]
      - ... continues to tags[num_tags - 1]

  - result[1]

    - same as result[0]

  - ...continues to result[24] (since there are 25 results on a page unless it is the last page)
