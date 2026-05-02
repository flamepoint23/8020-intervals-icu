# 8020 to Intervals.icu

This project was created using bun but updated to work with native node TypeScript support in Node 24.15. The package manager used was pnpm. The platform was `win32` (Windows 11).

First, install dependencies:

```bash
pnpm i
```

Get your intervals.icu information from:

intervals.icu/settings >> Developer Settings >> (Athlete ID) and (API Key >> (view))

And place it in a `.env` file (rename [rename-me-to-.env](./rename-me-to-.env))

#### **`./.env`**

```
API_KEY=yourKeyHere
ATHLETE_ID=yourAthleteIdHere
```

To pull the links for the workouts:

```bash
pnpm scrape
```

To download all the fit files into folders by sport:

```bash
pnpm down
```

> :warning: **This command triggers several API requests that modify your intervals.icu workout library by creating workout folders and uploading 479 workouts to your libary**: keep in mind that if you already have these workout folders populated, duplicates will be uploaded.

```bash
pnpm upload
```
