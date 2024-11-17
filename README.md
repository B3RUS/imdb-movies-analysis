# imdb-movies-analysis
Movie analysis on IMDb to see which movies from the last 5 years are worth watching.

The idea came from noticing (in my opinion) a decline in the quality of movies in recent years. However, I can't rely solely on intuition, so it would be worth checking if this is reflected in the data. After quickly browsing the Filmweb portal, I noticed that there are few movies with a rating higher than 7/10.

### What we want to know?

- How many movies have a rating higher than 7/10?
- How many of these movies are remakes or sequels?
- Seasonality of movie genres - in which month are there the most horror movies, etc.?

### Technical Preliminary Assumptions

First things first, we will use the API provided by https://www.omdbapi.com/ for convenience, which provides data from the IMDb portal in a simpler form. The limitation is the free API, which restricts us to retrieving 1000 data points per day.

Classically, we need to build a database of movies first. Clean them, and only then can we proceed to analysis. We will analyze using Python, Jupyter, and Matplotlib.