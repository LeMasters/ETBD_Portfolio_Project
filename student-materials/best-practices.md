# Portfolio Site: Best Practices

21 Nov 2026 · Garrison LeMasters

Your site is read quickly, often on a phone. Light, well-sized images and short, specific captions do more for it than any design change.

## Photos at a glance

Export project images at **1800 × 1200 pixels (3:2), under about 400 KB each**. Alexander, the class template, makes smaller copies for phones and laptops itself, so you upload one well-sized original; a straight-from-camera photo several times larger only slows each rebuild.

| Image (form) | How the page shows it | Export at | Aim for |
| --- | --- | --- | --- |
| Project image (Selected Work) | A card on the home page (3:2; a wide card shows about the middle 60% of a 3:2 image's height, or a squarer image whole); whole, uncropped, on the project's own page | 1800 × 1200 px, 3:2 | Under about 400 KB |
| Section pictures (Selected Work, Sections) | Whole, about half the page wide, beside a block of text | Any shape, up to 1600 px on the long side | Under about 300 KB |
| Gallery image (Gallery) | A square crop in the gallery grid; whole on its own page | Any shape, up to 2000 px on the long side | Under about 500 KB |
| Résumé (Profile) | Downloaded, not shown | PDF | Under 1 MB |

Why larger than the display size: phones and many laptops have high-density screens that use two pixels for each one on the page, and the wide feature card spans the whole page. Alexander publishes copies up to 2000 px wide, never wider than your original; beyond the sizes above, extra pixels add weight and no sharpness.

Use **one shape for all project images**: 3:2 landscape. Small cards share fixed 3:2 frames, so another shape is cropped to fit; a wide card shows a squarer image whole. Keep titles, HUD and faces away from the top and bottom edges. Gallery and section pictures can be any shape.

## Exporting photos and screenshots

Any editor that can resize and export will do: Lightroom, Photoshop, Affinity, GIMP, macOS Preview, or the free web tool Squoosh (squoosh.app).

1. **Crop first**, to the shape the page uses: 3:2 for project images.
2. **Resize** to the pixel size in the table above.
3. **Choose the format:**
   - **JPEG** for photographs and 3D renders. Quality 75–85 is usually indistinguishable from 100 at a fraction of the size.
   - **PNG** for screenshots with interface text, flat-colour art and pixel art, where JPEG blurs sharp edges. Scale pixel art by a whole number (2×, 3×, 4×) with "nearest neighbour" resampling so pixels stay square.
4. **Use the sRGB colour profile**, so colours look the same in every browser.
5. **Check the file size** before uploading. Over the target? Lower the JPEG quality a step, or reduce the pixel size.

Game screenshots: capture at the resolution you play at, then resize down. Pick frames that show the mechanic you're describing, not only the title screen.

## Files and names

- **Name files plainly before uploading,** with words that say what it is: `lantern-hours-level-2.jpg`, not `IMG_4471 (1).JPG`. Alexander turns spaces and unusual characters into underscores in the published copies; the words still show in your site's addresses and in what search engines see.
- **Résumé:** a PDF under 1 MB, exported from your editor (not a scan or a phone photo). Leave the field empty and the résumé link disappears.
- **Replacing an image** in a form uploads a new file; the old one stays stored in your repository. That does no harm to the page.

## Writing for the page

These apply the class's *Prototype Guidelines for ETBD Games Portfolio (INTERNAL)* to Alexander's fields.

| Field (form) | Aim | Example |
| --- | --- | --- |
| Area of expertise (Profile) | Say what work you want, in one line | "Level designer and playtester" |
| About (Profile) | Who you are, what you make, what you're looking for next, in two to four sentences | "I design puzzle levels and run playtests. Looking for a junior level-design role from June 2027." |
| Caption (Selected Work) | What it is and what you did, in one line | "Puzzle game · Unity · level design, team of four" |
| Description (Selected Work) | Role, tools, problem solved, outcome; for a case study, Sections that tell the story | "Designed four puzzle levels in Unity; reworked two after playtests showed players missed the light mechanic." |
| What you did (Experience) | Start with a verb; one result per sentence | "Ran weekly playtests and turned notes into design changes." |
| Note (Tools) | General only: how long, how much, what kind of work. It shows under the tool on your home page, so leave single-project details for that project's Sections | "C#; three years" or "Used on two team projects" |

- **Three strong projects beat ten.** Put your best and most recent first: Order 1 becomes the wide feature at the top of your home page.
- **Every image needs words.** A visitor who has never seen your game should know what they're looking at and why it's there.
- **Cut what repeats.** If a project shows nothing the others don't, consider leaving it out.

## Links and testing before you share

- **Type full addresses, starting `https://`.** Alexander adds a missing `https://` for you, but a typo still leads nowhere.
- **Link to your account of the work:** your itch.io page, a playable build, a trailer. Avoid links that send a reader away to someone else's description.
- **Test like a reviewer:**
  - [ ] On a phone, top to bottom, and on someone else's computer
  - [ ] On a slow connection (phone data, not campus Wi-Fi)
  - [ ] Every link and button clicked once
  - [ ] Your name visible at the top as you scroll
  - [ ] No sample text or placeholder images left
  - [ ] Your address pasted into a message to yourself, to see the preview others will see
