# Bridger Bowl live weather screenshot

Takes a screenshot of https://bridgerbowl.com/weather/live#Boundaries every
30 minutes using [shot-scraper](https://github.com/simonw/shot-scraper) and
GitHub Actions (structure based on simonw/shot-scraper-template).

Each run replaces the previous image. It is published to a single-commit
branch named `latest`, so the URL never changes:

    https://raw.githubusercontent.com/<USER>/<REPO>/latest/boundaries.png

Note: raw.githubusercontent.com caches for about 5 minutes.

## Files

- `shots.yml` - what to capture (URL, size, wait, output file name)
- `.github/workflows/shots.yml` - the schedule and publish step
- `requirements.txt` - installs shot-scraper

## Run manually

Actions tab > "Take screenshot" > Run workflow.
