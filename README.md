# mindwank.com

The personal website of Mind Wank, an "artist" who uses "AI". Plain HTML and
one shared stylesheet. No frameworks, no build step, no analytics.

## File structure

```
index.html        home page: the whole site index, one list going down
about.html        bio and portrait (not linked from the home page)
cv.html           exhibitions, awards, press
contact.html      email, commissions, socials (not linked from the home page)
404.html          not found page
styles.css        the only stylesheet
favicon.ico       placeholder favicon
netlify.toml      404 redirect rule for Netlify
img/              og.png and portrait.png, gray placeholders to be replaced
                  with real images under the same filenames
```

## Deploying

This is a static site with no build step. On Netlify, create a site from this
repository, leave the build command empty, and set the publish directory to the
repository root. The included `netlify.toml` serves `404.html` for unknown
paths. To update the site, replace the placeholder files in `img/` with real
images under the same filenames, edit the HTML, and push. That is the whole
pipeline.
