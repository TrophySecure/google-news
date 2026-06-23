[Google News](https://apify.com/canadesk/google-news?fpr=data)

⏰ Want to schedule this actor to run on a regular basis? Check [https://docs.apify.com/platform/schedules](https://docs.apify.com/platform/schedules)!

## Input

- Topics (select)

- All: Runs all below topics.
- Top Stories: Headlines, equivalent to "Home".
- Country & World: Country is based on the selected user region.
- Others: Equivalent to the default categories on Google News, such as Business, Technology, Entertainment, etc.
- Custom Topic (string)

➡ **Overrides** "Topics". Equivalent to the search bar (free text).

"Include related articles" and "Search Text" are not supported here.
- Pagination (select)

- Latest: First articles displayed before pagination.
- All: Equivalent to "Load more".
- Include related articles (select)

Will find relevant news associated with each article.
- Region (select)

💡 Simulates the user geolocation. Most of the results are based on this input.
- Search text (string)

Filter applied AFTER data collection. Only returns news containing the search text.
- Period (select)

Filter applied AFTER data collection. Only returns news within the timeframe (UTC!).

## Example

```
{
	"others": [
		{
			"id": "CAAqJggKIiBDQkFTRWdvSUwyMHZNRGRqTVhZU0FtVnVHZ0pWVXlnQVAB",
			"name": "Technology",
			"articles": [
				{
					"title": "Sketchy Nintendo Switch 2 listing reveals the gaming handheld's pre-order price",
					"short": "While the Nintendo Switch 2 was fully showcased, its official price still remains a mystery. Ahead of any official words from the company, a lesser-known...",
					"source": "Notebookcheck.net",
					"timestamp": 1737803700000,
					"datetime": "2025-01-25T08:15:00.000Z",
					"url": "https://www.notebookcheck.net/Sketchy-Nintendo-Switch-2-listing-reveals-the-gaming-handheld-s-pre-order-price.952304.0.html",
					"image": "https://news.google.com/api/attachments/CC8iK0NnNW1URmMyVEVKRGJqZEtWVGR4VFJEZkF4aUFCU2dLTWdZUmtwUXFNUWM=s0-w100-h100-p-rw-df",
					"related": [
						{
							"title": "This ‘Light Mode’ Switch 2 Is Stunning, But There’s A Catch",
							"short": "They say software sells hardware. But there's a secondary motivator that will make the Switch 2 fly off the shelves, and that's the perfect splash of color.",
							"source": "Forbes",
							"timestamp": 1737818504000,
							"datetime": "2025-01-25T13:15:04.000Z",
							"url": "https://www.forbes.com/sites/jasonevangelho/2025/01/25/this-light-mode-switch-2-is-stunning-but-theres-a-catch/",
							"image": "https://news.google.com/api/attachments/CC8iI0NnNXBOblJrYVdFNVFXeFdXSFJPVFJDZkF4ampCU2dLTWdB=s0-w100-h100-p-rw-df"
						},
						{
							"title": "Some Mario Kart 9 fans are less concerned about whether or not the racer will be Nintendo Switch 2's launch title than they are about its name",
							"short": "Mario Kart 2? Mario Kart X? Mario Kart 8 Deluxe 2? The possibilities are (somewhat) endless.",
							"source": "Yahoo! Voices",
							"timestamp": 1737559857000,
							"datetime": "2025-01-22T13:10:57.000Z",
							"url": "https://www.yahoo.com/tech/mario-kart-9-fans-less-153057163.html",
							"image": "https://news.google.com/api/attachments/CC8iK0NnNXBXRTFsZDJSVFZtRklhM0ZZVFJDZkF4ampCU2dLTWdZbGdvNnR0UVU=s0-w100-h100-p-rw-df"
						},
						...
					]
				},
			],
		},
		...
	]
}
```

## Support

Always use a strong proxy!

Open a new issue for bugs, please share your Run URL and Input 🎈