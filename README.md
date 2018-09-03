# frontend-ajax-examples

Credit to Pamela Fox: https://gist.github.com/pamelafox/3926362

Exercise: Nutrition Facts

    Create an empty webpage.
    Download nutrition.xml from https://gist.github.com/3000322 and place in your project folder.
    Use AJAX via jQuery or JS API to fetch the file into the page.
    Create a table. For each <food> in the XML file, create a row in the table with the food name and nutritional facts - serving size, calories, carbs.
    Bonus: Use the tablesorter jQuery plugin to make the table sortable by the nutritional facts.

Exercise: Lady Gaga News

    Create an empty webpage.
    Download the RSS feed at http://www.ladygaga.com/feeds/artist/content/ and store it in your project folder.
    Use AJAX (via the raw JS API or jQuery) to load the file into your page.
    Create a <h1> with the title of the RSS feed.
    Create a <ul>. For each <item>, create a <li> which contains the title and date of the post, and is linked to the post.
    Bonus: Use moment.js to pretty-print the date posted ("3 hours ago"). 

Exercise: Roomie Shopping List
*Has to be done with a regular Gmail account, not Google Apps

    Create a new Google spreadsheet.
    Add columns for “item”, “quantity”, and “requestor”.
    Add 5 rows (whatever your fridge is missing!).
    Publish the spreadsheet (via File->Publish as webpage).
    Use the JSONP technique to bring the published feed into your page as JSON.
    The URL should be of this form: https://spreadsheets.google.com/feeds/list/o03712292828507838454.2635427448373779250/od6/public/basic?alt=json-in-script&callback=listTasks

    The URL is like:

http://spreadsheets.google.com/feeds/list/{SPREADSHEET_KEY}/{WORKSHEET_ID}/
public/basic?alt=json-in-script&callback={callbackName}

The spreadsheet key is usually in the URL, the worksheet ID is always od6 for the first worksheet, and callback name is whatever your function is called.

    Create a <ul> with each shopping item as an <li>.
    Bonus: Use the Google Image Search API to find an image for each item.

Exercise: Seattle Restaurants

    Create an empty webpage.
    Download the XML file at https://gist.github.com/3000348 and store in your project folder.
    Use AJAX (via raw JS API or jQuery) to load the file into your page.
    Create a <ul>. For each <restaurant>, create an <li> with the name and address of the restaurant. Change the color of the text depending on the type of the restaurant (“sitdown” or “bar”).
    Link each address to Google Maps.
    Bonus: Use the Google Static Maps API to render a map for each restaurant.


Exercise: Gaga Tweets

    Start with the webpage from the Gaga RSS exercise.
    Figure out the URL that will load in the latest tweets from LadyGaga (hint: https://dev.twitter.com/docs/api/1/get/statuses/user_timeline). Test in the browser to see what the JSON looks like.
    Use either raw JS or a library to load the JSON into the page.
    Create a <ul> with an <li> for each tweet. The <li> should contain the text and the time, where the time is linked to the individual tweet on twitter.com

    Bonus: Use moment.js to pretty-print the date posted ("3 hours ago"). 

    Bonus:  Combine the news and tweets into the same <ul>, sorted by time.
