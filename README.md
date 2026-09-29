# maxgallop.com

Jekyll site, built and hosted by GitHub Pages. Nothing to install locally.

## Adding or updating a paper
Edit `_data/papers.yml`. Titles link to `url:` (open-access versions preferred), falling back to the DOI. The research page is generated from it; the field
list is at the top of the file. Entries show in the order listed.

## Current projects
Entries with `status: project` appear under "Current projects" at the top of
the research page. Fill in `summary:` (1-2 sentences) for each; it is left out
while empty. A project without a paper can link talk slides via `slides:`.
When a project is published, change its status to `article` and add the venue.

## Adding a figure
Put the image in `images/` using the filename already listed in the paper's
`image:` field. It appears on the next build; entries without a file show
without a figure. Any size or aspect ratio works; white backgrounds are best.

Optional: to keep a caption off the small thumbnail, put a cropped copy with
the same filename in `images/thumbs/`. The page shows the cropped copy and
clicking opens the full image (with caption) from `images/`.

## Updating the CV
Replace `cv.pdf`.

## Going live
1. Create a GitHub repository and push this folder to it.
2. Repository Settings > Pages: deploy from the main branch, root folder.
3. At your domain registrar, point maxgallop.com at GitHub Pages
   (A records for the apex domain, CNAME for www), using the addresses in
   GitHub's "Managing a custom domain" documentation.
4. Back in Settings > Pages, confirm the custom domain and tick "Enforce HTTPS"
   once the certificate is issued.

## Style
Colours are set as tokens at the top of `assets/style.css` (light and dark
mode). An alternative header-band style is parked in `_variants/header-band.css`;
Jekyll doesn't publish folders starting with an underscore, so it isn't live.
