# Timestamp Microservice  

You can run my code on the replit online IDE to check how it works:
https://replit.com/join/ndqvyoagvq-kamilsynowiec

- A request to /api/:date? with a valid date returns a JSON object with a unix key that is a Unix timestamp of the input date in milliseconds.

- A request to /api/:date? with a valid date returns a JSON object with a utc key that is a string of the input date in the format: Thu, 01 Jan 1970 00:00:00 GMT

- A request to /api/1451001600000 returns { unix: 1451001600000, utc: "Fri, 25 Dec 2015 00:00:00 GMT" }

- If the input date string is invalid, the api returns an object having the structure { error : "Invalid Date" }

- An empty date parameter returns the current time in a JSON object with a unix key (a request to /api)

- An empty date parameter returns the current time in a JSON object with a utc key
