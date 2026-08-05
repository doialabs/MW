# mindwank.com

The personal website of Mind Wank, an "artist" who uses "AI". Plain HTML and
one shared stylesheet. No frameworks, no build step, no analytics.

## File structure

```
index.html        home page
about.html        bio and portrait
cv.html           exhibitions, awards, press
gallery.html      artwork index
gallery-1.html    Artwork I
gallery-2.html    Artwork II
gallery-3.html    Artwork III
gallery-4.html    Artwork IV
contact.html      email, commissions, socials
404.html          not found page
styles.css        the only stylesheet
favicon.ico       placeholder favicon
netlify.toml      404 redirect rule for Netlify
img/              image files, one per work, named after the piece (equus.png,
                  domesticity.png, etc.), plus og.png and portrait.png. The
                  committed files are gray placeholders: drop in the real
                  artwork under the same filenames to replace them
```

## Deploying

This is a static site with no build step. On Netlify, create a site from this
repository, leave the build command empty, and set the publish directory to the
repository root. The included `netlify.toml` serves `404.html` for unknown
paths. To update the site, replace the placeholder files in `img/` with real
artwork (keeping the same filenames, or updating the `src` attributes in the
gallery pages), edit the HTML, and push. That is the whole pipeline.
