# serena-lee-website

One-page portfolio site for Serena Lee, a freelance wedding and portrait photographer.

Plain HTML and CSS, with a dark theme. There is no build step and no dependencies.

## Files

- `index.html`: the whole page, with styles inline
- `wedding-01.png`: portfolio photo, first frame
- `vercel.json`: Vercel settings (static output, clean URLs, security and cache headers)

## Deploy on Vercel

1. In Vercel, choose **Add New > Project** and import this repository.
2. Leave the framework preset as **Other**. Leave the build command and output directory empty (`vercel.json` already sets them).
3. Select **Deploy**. Every push to `main` redeploys the site.

Or from the terminal:

```
npx vercel        # preview deployment
npx vercel --prod # production deployment
```

## Preview locally

```
npx serve .
```

## Add photos

Put each image in this folder and place it in a frame in `index.html`:

```html
<div class="frame"><img src="your-photo.jpg" alt="Describe the photo" width="1200" height="1500"></div>
```

Frames crop to a 4:5 portrait shape. Remove the matching `t1` to `t6` class once a frame has a photo.

## Before going live

- Replace `hello@serenalee.com` with Serena's real email address (two places in the contact section).
- Edit the about text to her own words.
