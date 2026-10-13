# Movie Recommendation System

A fully client-side **content-based movie recommender**.

## Live app

**https://movie-recommendation-system-two-eta.vercel.app/**

## What changed

The repository previously had no implementation. It now contains a working interactive recommender.

Choose one movie and the application ranks the most similar titles using:

- genre overlap
- theme/keyword overlap
- release-era similarity

Everything runs locally in the browser.

## Recommendation logic

Each movie has a set of content tags.

The recommender calculates tag overlap using a Jaccard/cosine-style similarity score and adds a small release-era similarity component.

```text
selected movie
   -> compare content tokens
   -> calculate overlap score
   -> compare release year
   -> rank remaining movies
   -> show best matches
```

## Features

- Interactive movie selector
- Eight ranked recommendations
- Similarity percentage
- Genre/theme tags
- No API key
- No database
- No backend
- Deterministic results

## Run locally

```bash
cd web
python -m http.server 8000
```

Open:

```text
http://localhost:8000
```

## Tech stack

- HTML
- CSS
- Vanilla JavaScript
- Content-based filtering
- Vercel

## Scope

The included dataset is intentionally small and embedded in the demo. It demonstrates recommendation-system logic rather than claiming production-scale personalization.

A production recommender would normally use a larger catalog, user behavior, offline evaluation and feedback loops.

## Author

**Sankalp Gupta**

GitHub: https://github.com/Sankalp-gupta1
