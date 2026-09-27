# For Diya ♡ — apology website

A responsive, static romantic apology page built with HTML, CSS, and vanilla JavaScript. No backend or build step is required.

## Preview locally
1. Unzip this folder.
2. Open `index.html` in a modern browser.

## Replace the six photo placeholders
Inside `index.html`, find the `photo-row` and `memory-grid` sections. Each placeholder looks like:
```html
<div class="photo"><span>📷<br>Photo 1<br><small>Replace with our photo</small></span></div>
```
Replace the inner `<span>...</span>` with an image tag, for example:
```html
<img src="images/our-photo-1.jpg" alt="A favorite photo of us">
```
Create an `images` folder beside `index.html`, then put your images there. Keep the image aspect ratio portrait; CSS uses `object-fit: cover`.

## Free hosting
### Netlify
1. Visit https://app.netlify.com/drop
2. Drag the unzipped project folder (containing `index.html`) onto the page.
3. Netlify will publish it and provide a shareable URL.

### GitHub Pages
1. Create a GitHub repository and upload `index.html` (and your `images` folder, if used).
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. Wait for the published site URL shown in Pages.

## Interaction notes
- YES and NO begin side by side. NO remains stationary.
- YES glides away when the pointer gets close; its movement is bounded to the viewport.
- On touch, tapping YES triggers a gentle escape attempt. NO remains easy to tap.
- The six photo placeholders are intentionally static, not a carousel.
