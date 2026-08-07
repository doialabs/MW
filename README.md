# mindwank.com

The personal website of Mind Wank, an "artist" who uses "AI". Plain HTML and
one shared stylesheet. No frameworks, no build step, no analytics.

## File structure

```
index.html        home page: the whole site index, one list going down
cv.html           exhibitions, awards, press contact
404.html          not found page
styles.css        the only stylesheet
favicon.ico       placeholder favicon
netlify.toml      redirects from old Squarespace URLs, plus the 404 rule
img/              og.png, a gray placeholder to be replaced with a real
                  image under the same filename
```

## Deploying

This is a static site with no build step. On Netlify, create a site from this
repository, leave the build command empty, and set the publish directory to the
repository root. The included `netlify.toml` serves `404.html` for unknown
paths. To update the site, replace the placeholder files in `img/` with real
images under the same filenames, edit the HTML, and push. That is the whole
pipeline.
