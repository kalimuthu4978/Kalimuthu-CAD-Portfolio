# Sathishkumar — portfolio profile

Portfolio page built from Sathishkumar's résumé. It will be
published at `<site>/sathishkumar/` and reuses the main site's `styles.css`.

## Where to put your files

- `assets/resume/`: the résumé PDF for this profile (plus a .docx if you have one)
- `assets/projects/`: project images, **one subfolder per project**, e.g.
  - `assets/projects/Turbine Blade/scan.png`
  - `assets/projects/Turbine Blade/cad.png`
- `assets/photos/`: any other images (field work, setups, headshot)

Name the files as you like, but don't rename them once the page is built:
GitHub Pages treats file names as case-sensitive.

Before publishing, remove customer names, part numbers and any other
proprietary details from the images.

## Web images

The page loads the WebP copies in `assets/web/thumb/` (cards, 640 px) and
`assets/web/full/` (gallery, 1600 px), not the originals in `assets/projects/`
(about 243 MB of PNGs). After adding or replacing a project image, regenerate the
copies and add the project to the `projects` list in `index.html`.

## Local preview

From the repository root (so `../styles.css` resolves):

    python -m http.server 8080

then open http://127.0.0.1:8080/sathishkumar/
