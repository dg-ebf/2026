# DG-EBF CVPR 2026 Workshop Website (Design v4)

Design direction: **Editorial / conference brochure** — clean light theme, big images, minimal chrome.

This version:
- Keeps the **same content arrangement** as the 2025 website (Home: Motivation → Invited Speakers → Organizers → Topics → Paper Submission → Contact → Sponsors).
- Adds **big image tiles** for speakers and organizers (like last edition), using placeholder SVGs you can swap with real photos.

## Replace placeholder images
Put a headshot at:
`images/people/<name-slug>.jpg` and update the corresponding `<img src="...">` in `index.html` / `organizers.html`.
The cards are already styled with `object-fit: cover` for large, clean crops.

## Files
- index.html
- call-for-papers.html
- program.html
- organizers.html
- styles.css
- script.js
- images/hero.svg
- images/people/*.svg
## Speaker images (filenames already wired)
Place/replace these files in `images/people/`:

- sara_beery_512.jpg
- aditi_raghunathan_512.jpg
- kun_zhang_512.jpg
- m_saquib_sarfraz_512.jpg
- abhinav_dhall_512.jpg
- zsolt_kira_512.jpg

## Previous edition
The nav includes a 'Previous Edition' link to: https://cvpr25workshop.m-haris-khan.com/

## No-crop speaker photos
Cards use `object-fit: contain` with `max-width/max-height` so headshots are never cropped. Adjust `.media` height/padding in `styles.css` if needed.


## Square (512×512) photos
This version assumes all speaker/organizer photos are square (e.g., 512×512). Speaker tiles use `aspect-ratio: 1/1` and `object-fit: cover` so photos fill the tile without cropping.
