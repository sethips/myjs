
# myjs
A simple JavaScript Facade library, to facilitate my life.

[![](https://data.jsdelivr.com/v1/package/gh/assisfery/myjs/badge)](https://www.jsdelivr.com/package/gh/assisfery/myjs)

## Demo
See the demo here: [https://assisfery.github.io/myjs/index.html](https://assisfery.github.io/myjs/index.html)

## Cookies
To manage cookies use those functions.

Set a value to cookie.
```js
myjs.setCookie(key, value)
```

Set a value for a cookie with expiration days.
```js
myjs.setCookie(key, value, days)
```

Get a defined cookie.
```js
myjs.getCookie(key)
```

Verify if a cookie exists.
```js
myjs.hasCookie(key)
```

Delete a cookie.
```js
myjs.removeCookie(key)
```

## Query String
To get query string parameters from url you can use that function.

Get query string from current page url.
```js
myjs.getQuery(key)
```

Get query string from a url.
```js
myjs.getQuery(key, url)
```

## Validations
To validate some data use those functions.

To validate if a string is email.
```js
myjs.isEmail(str)
```

To validate if a string is URL.
```js
myjs.isUrl(str)
```

To validate if a string is a number.
```js
myjs.isNumber(str)
```

## Slugify
To slugify a string use that function.

Return a string slug.
```js
myjs.slug(str)
```

## Random
To get the random number use that function.

Get a random number from min to max, but max is not included.
```js
myjs.random(min, max)
```

Get a random number from zero to max, but max is not included.
```js
myjs.random(max)
```

## Navigator
To execute navigator utils use that functions.

Redirect page to another url.
```js
myjs.redirect(url)
```

## Element
To manipulate dom use those function.

Get all elements that match with query done. For example: myjs.e(".btn") will select all elements that has class "btn".
```js
myjs.e(query)
```

Add a class to all elements that match with query.
```js
myjs.addClass(query, class)
```

Remove a class to all elements that match with query.
```js
myjs.removeClass(query, class)
```

Set a inner html in all elements that match with query.
```js
myjs.setHtml(query, html)
```

Get a inner html of the first element that match with query.
```js
myjs.getHtml(query)
```

## DrawChart
To draw a chart you can use those functions.  

Those functions depends of ChartJS libray.

To draw a simple chart of any type supported by ChartJS.
```js
 myjs.drawChart(area, type, title, labels, data)
```
Sample
```js
myjs.drawChart('#chart1', 'bar', 'Some chart', ['A', 'B', 'C'], [1, 2, 3])
```

To draw a series chart of any type supported by ChartJS.
```js
myjs.drawChartSerie(area, type, labels, datasets)
```
Sample
```js
myjs.drawChartSerie('#chart2', 'bar', ['A', 'B', 'C'],
	[
		{
           label: 'Some data 1',
           data: [12, 19, 3],
           backgroundColor: myjs.purpleColors,
           borderColor: myjs.purpleColors,
           borderWidth: 1
       },
       {
           label: 'Some data 2',
           data: [2, 6, 8],
           backgroundColor: myjs.blueColors,
           borderColor: myjs.blueColors,
           borderWidth: 1,
       }
	]
);
```


## Local Storage
To use localStorage, for storing data in your browser, use those functions.

Set a value to localstorage.
```js
 myjs.setLocal(key, value)
```

Get a defined localstorage.
```js
myjs.getLocal(key)
```

Verify if a localstorage exists.
```js
myjs.hasLocal(key)
```

Remove localstorage data.
```js
myjs.removeLocal(key)
```

## Sessions Storage
To use sessionStorage, for storing data in your browser, use those functions.

Set a value to sessionStorage.
```js
myjs.setSession(key, value)
```

Get a defined sessionStorage.
```js
myjs.getSession(key)
```

Verify if a sessionStorage exists.
```js
myjs.hasSession(key)
```

Remove sessionStorage data.
```js
myjs.removeSession(key)
```