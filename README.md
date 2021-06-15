# How Does a YouTube Video Go Viral

Demo for YouTube videos and channels using Chart.js.

## Installation

There is **no need for installation**. Instead, take the files and open them in your favorite browser. We use JSONP to provide data inside the script; some browsers might block those requests. If there is any error, check the console.

## Dataset

All the video data is in the `data.jsonp` file. The data comes directly from a [ZenRows](https://www.zenrows.com/) Task. We removed some fields to make it smaller. The script supports datasets with all the fields, so do not worry about directly pasting a new task output. Just be careful with its size, a huge file can freeze your browser.

In the HTML file is a **minimum configuration** in case you want to change it and see different data. After setting the new data, modify the values inside `dataConfig` and refresh the page. Those should tell the script the minimum videos or views, the selected channel, etc...

### Chart.js and Luxon

Here we use some open-source projects for he charts: [Chart.js](https://www.chartjs.org), [Luxon](https://moment.github.io/luxon), [chartjs-adapter-luxon](https://github.com/chartjs/chartjs-adapter-luxon), and [Lodash](https://lodash.com). Thanks once again to all of them. There is more info about how it works in the [HTML file](./index.html).

## How to get your own data

We need a **simple structure**: an object array containing channelName, title, videoId, viewCount, and date (timestamp).

You can gather that information manually for small datasets, but that will get complicated for large sets. However, there are great ones published online and free-to-use. Feel free to check them out and test them.

For **people with data or content**, export or transform them as JSON. [MySQL](https://dev.mysql.com/doc/mysql-shell/8.0/en/mysql-shell-json-output.html) supports exporting to JSON/array, and the same goes for  [MongoDB](https://docs.mongodb.com/database-tools/mongoexport/). You can also get excel or CSV files and convert them. But, again, there are online tools for that.

### How to collect online data

We implement a **no-code solution** for those of you that have great ideas but no data. You can several URLs to get content from, and we will extract structured data and store it in any format, like JSON, for you. So give it a try in [ZenRows](https://app.zenrows.com/register).

We generated data for this with a simple recurrent task that *extracts data from several YouTube channels every 30 minutes**. It runs every time in just a few seconds.

If you like the results, get in [contact](https://www.zenrows.com/contact) to show us what you've done ;)

## Contributing
Pull requests are welcome. For significant changes, please open an issue first to discuss what you would like to change.

## License
[MIT](./LICENSE)
