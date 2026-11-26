# Cherin 

## Description

I would like to make an interactive exploration of my personal spotify data as a series of rings (inspired by visualcinnamon) where each ring is a slice of time and the color is music descriptive data like genre / artist / listening frequency. 

I want to answer questions like:
When in the day and the week do I listen, and does it differ by genre?
How did my taste shift over the years I have data for?

## Technical Plan re: Option A/B/C/D

Option A using D3.js

My idea is one major / large visualization with different ways of reconfiguring it with the user changing the encoding, data filter and compares scenarios. 

Libraries: 
- D3.js for scales, polar layout, arcs, transition
- Python (pandas) for cleaning and aggregating the raw Spotify export into a compact JSON/CSV

I am taking inspiration from spotify wrapped (year end listening summaries) and this piece from visualcinnamon (https://www.visualcinnamon.com/art/gdqs/).


## Mockup

![Prototype](interactive_data_viz_draft.png)

## Data Sources

{
include 1-3 data sources with the following,
you may re-use data sources from before or switch topics
}

### Data Source 1: Personal Spotify data

URL: https://support.spotify.com/us/article/understanding-your-data/

Size: unsure yet - will either be data from the the entire history of spotify that I have or from the past year. If anything I will look at example spotify profiles or have a third party give me listening data.

https://www.statsforspotify.com/

### Data Source 2: Artist genre tags

URL: https://developer.spotify.com/documentation/web-api (Spotify Web API artist metadata), with https://musicbrainz.org/doc/MusicBrainz_API or https://www.last.fm/api as backups

Size: one row per unique artist in my history (roughly 100 artists), a few columns (artist, list of genres)

## Questions

{Numbered list of questions for course staff, if any.}

1. Is a compare mode (two years or two artists side by side) enough on its own to count as "significant" interactivity, or would you want additional features?