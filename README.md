# Ethan's Bird Blog

Minimal white-background bird blog with a stacked archive of square image posts.

## Open The Website

### Option 1: Open it directly

Open `/mnt/d/Coding/Ethan's Bird Blog/index.html` in any web browser.

### Option 2: Run a local server

```bash
cd "/mnt/d/Coding/Ethan's Bird Blog"
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Main Files

- `index.html` is the archive page
- `about.html` is the separate about page
- `post.html` is the single-post page
- `SandHilledCranePost.js` stores the Sand Hilled Crane post content
- `SawWetPost.js` stores the Saw Wet Owl post content
- `posts.js` collects the post files for the site
- `app.js` renders the archive list
- `post.js` renders an individual post
- `styles.css` controls the site design
- `assets/Photos/` stores the original bird images
- `assets/Web/` stores the optimized web images used by the live site

## Add Or Edit Posts

Open `SawWetPost.js` to edit the owl post title, description, date, and images.
Open `SandHilledCranePost.js` to edit the crane post title, description, date, and images.

The main description text is inside the `body` array.

For each post, edit:

- `slug`
- `title`
- `date`
- `year`
- `location`
- `image`
- `alt`
- `summary`
- `body`

To use your own bird photos:

1. Put the image inside `assets/`
2. Change the `image` or `images` paths in `SawWetPost.js`

If you add more posts later, you can create more files like:

- `SandHilledCranePost.js`
- `SawWetPost.js`
- `CardinalPost.js`
- `HeronPost.js`

Example:

```js
window.SAW_WET_POST = {
  slug: "northern-cardinal-at-sunrise",
  title: "Northern Cardinal At Sunrise",
  date: "April 2, 2026",
  year: "2026",
  location: "Backyard Fence",
  image: "assets/cardinal.jpg",
  alt: "Northern cardinal perched on a wooden fence at sunrise.",
  summary: "A bright red flash landed just as the morning light came through the trees.",
  body: [
    "The cardinal arrived early and stayed just long enough to catch the first warm light.",
    "It turned an ordinary fence into the whole reason to stop and look."
  ]
};
```
