# Movie Recommendation System

A live, explainable **content-based movie recommendation** demo.

## Live app

**https://movie-recommender-sankalp.vercel.app/**

## What the project does

Choose a movie you like and the app recommends five similar titles.

The score uses:

- shared genres,
- shared mood tags,
- release-year similarity,
- runtime similarity.

You can also filter recommendations by genre or mood.

## Why this implementation is transparent

The repository originally had documentation but no implementation files.

The deployed version therefore does not pretend that an older hidden model exists. It uses a small curated movie catalogue and an explainable content-similarity algorithm implemented directly in JavaScript.

## Tech stack

- HTML
- CSS
- JavaScript
- Content-based recommendation
- Vercel

## Run locally

```bash
cd web
python -m http.server 8000
```

Open `http://localhost:8000`.

## Limitations

- The demo uses a small built-in movie catalogue.
- It does not use personal viewing history.
- It is not a collaborative-filtering production recommender.
- The ranking is deterministic and designed to be easy to inspect.

## Author

Sankalp Gupta  
GitHub: https://github.com/Sankalp-gupta1
