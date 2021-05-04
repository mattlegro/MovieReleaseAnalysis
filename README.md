# Phase 1 Project

This repo is a collection of notebooks and resources used to conduct the following project.

## Business Problem

* Global Box Office Revenue hit a new record in 2019 at $42.5 billion and has been growing every year
* Netflix is reported to invest $15 billion on new content; Prime Video and Apple TV+ at $6 billion; Hulu, Disney+ and HBO Max are all   coming in around $3 billion
* Enable Microsoft to join the media industry as a production company and grow shareholder value
* Determine features of successful theatrical movie releases to guide Microsoft in producing films that will generate profit

## The Data

In the folder `zippedData` are movie datasets from:

* [Box Office Mojo](https://www.boxofficemojo.com/)
* [IMDB](https://www.imdb.com/)
* [Rotten Tomatoes](https://www.rottentomatoes.com/)
* [TheMovieDB](https://www.themoviedb.org/)
* [The Numbers](https://www.the-numbers.com/)

From these files, the following tables were used to build a dataset, saved in dataFiles as movie_collection.
* imdb.title.basics
* imdb.title.ratings
* imdb.title.principals
* tmdb.movies
* tn.movie_budgets

Additional data, including the IDMb unique identifier (found in the data as tconst), was added to the tmdb.movies data table by using the id column, which is a unique identifier for their database, to query the TMDb API. A tconst was assigned to all movies in the TN dataset, whereupon other information was assigned to each record from the listed IMDb tables.

These two tables were then concatenated and duplicates removed, resulting in a collection of ~2370 movies with fields:
> 'tconst', 'Title', 'Genres', 'runtime_minutes', 'vote_average','vote_count', 'budget_est', 'worldwide_gross', 'release_week_day',
> 'release_day', 'release_month', 'release_year'

## The Questions

### How much should Microsoft spend?

### How should the production budget be invested?

### When should the film be released?

## Summary

### Our Conclusions

### For Future Research
