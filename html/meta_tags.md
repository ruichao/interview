# Meta tags

The `meta` tags generally describes information about HTML page. It also be used to emulate an HTTP response header and it has attributes like `http-equiv` and `charset`.


## Name attribute

### keywords and description

Google (announced in 2009) doesn't use meta keywords or descriptions in their search algorithms for ranking purposes.

The `description` meta tags have no effect on search engine rank, they do appear in search results. Meta descriptions should be written for people to read rather than for robots to find.

```
<meta name="description"
      content="A general guide on the usage of meta tags>
```


```
<meta name="keywords"
      content="react, reudx, webpack">
```

### author

Set the author of a page

```
<meta name="author" content="kaka">
```

### viewport

```
<meta name="viewport" content="width=device-width,initial-scale=1"/>
```

### copyright (obsolete)

```
<!-- don't use this! -->
<meta name="copyright" content="SitePoint" />
```

instead: providing a link tag pointing to a copyright page

```
<link rel="copyright" href="copyright.html">
```

## charset

The `charset` attribute is used to specify the character encoding of your content.

```
<meta charset="UTF-8">
```

## http-equiv

meta tags can be used to perform the task of HTTP headers like redirection and refresh.

### refresh

```
<meta http-equiv="refresh" content="5,url=http://www.google.com">
```

The value of the content attribute refers to the time interval in seconds before the refresh is performed.

### expires

```
<meta http-equiv="expires" content="Fri,01Jan201618:18:18GMT">
```

Will re-fetch the page when it's expired (GMT format).

### Pragma

```
<meta http-equiv="Pragma" content="no-cache">
```

Disable browser to read data from cache

### Window-target

```
<meta http-equiv="Window-target" content="_blank">
```

Don't allow other people to include your pages into their own by iframe, frame, etc.


## Robots

```
<meta name="Robots" contect="...">
```

The content can be one of `none`, `noindex`, `nofollow`, `index`, `follow`, `all`.
