# unreal-case-studies

## Case 1 - Grab info from a public API in Unreal using authentication in VA Rest plugin

A colleague at SPI wanted to grab covid data from a public API so it could appear in his game. I'm happy to help with stuff like this

I felt like it was easiest to print to window before we applied to a game object (and a lot easier to test without events)

I grabbed a random test API from rapidAPI: https://rapidapi.com/Gramzivi/api/covid-19-data

Subscribed, grabbed the API key and host. The problem was the video tutorial he was working off of assumed there was no authentication, but you needed headers in the JSON GET request for rapidapi. This was easy enough to figure out on a Saturday after some googling.

Video tutorial https://www.youtube.com/watch?v=B90jnsEJ6E0
Call URL function was deprecated and changed to Apply URL. Applied Set Header functions, printed response.

![Alt text](varest.jpg?raw=true "VA Rest to grab public data")

Now my friend can call some Array handling and apply text wherever he likes according to events
