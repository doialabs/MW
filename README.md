# mindwank.com

The personal website of Mind Wank, an "artist" who uses "AI". Plain HTML and
one shared stylesheet. No frameworks, no build step, no analytics.

## File structure

```
index.html        home page: the whole site index, one list going down
cv.html           in-person exhibitions and awards, verbatim from the artist
404.html          not found page
styles.css        the only stylesheet
favicon.ico       quotation-mark favicon
vercel.json       redirects from old Squarespace URLs
img/              og.png, the social preview card
```

## Deploying

This is a static site with no build step. It deploys on Vercel: the repository
is linked to the Vercel project `mw`, and every push to `main` deploys
automatically. `vercel.json` redirects the old Squarespace URLs, and Vercel
serves `404.html` for unknown paths. To update the site, edit the HTML and
push. That is the whole pipeline.
