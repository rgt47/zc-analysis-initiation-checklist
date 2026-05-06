# Image Sources

*2026-04-29 13:40 PDT*

Attribution log for every image referenced from this post.
Update each entry when an image is added, replaced, or
removed.

## hero.jpg

- **Source:** Generated 2026-04-29 via Gemini (Imagen 3) at
  [gemini.google.com](https://gemini.google.com).
- **Prompt:** see Post 61 entry in
  `~/Dropbox/prj/qblog/HERO_IMAGE_PROMPTS.md`.
- **Processing:**
  `magick Gemini_Generated_Image_8qnai8qnai8qnai8.png
  -resize 1600x -strip -quality 85 hero.jpg`.
  Final dimensions 1600 by 893.
- **Description:** Editorial still life of a clean wooden
  desk with a printed multi-page checklist held under a
  brass paperweight, an open hardcover notebook with a
  fountain pen, a closed laptop, and a single sheet
  printed with a tabular grid (CSV-like).
- **Usage:** Hero image (80% width) immediately after the
  YAML block; also referenced in `image:` field of the
  blog post YAML.
- **License:** Generated content; no third-party rights.

## ambiance1.png, ambiance2.png, ambiance3.jpg

- **Status:** Placeholder. Inherited from the post-47
  template. Replace before flipping `draft: false`.
- **Replacement prompts:** see Post 61 entry in
  `~/Dropbox/prj/qblog/HERO_IMAGE_PROMPTS.md` (three
  prompts: ambiance image 1 after Objectives, ambiance
  image 2 mid-body, ambiance image 3 before Lessons
  Learnt).

## Template for Additional Images

When adding images to this post, use this format:

### image-name.jpg

- **Source:** [Generator + date, or photo source]
- **Prompt or attribution:** [link or full prompt]
- **Processing:** [exact magick / convert command if any]
- **Description:** [what the image shows]
- **Usage:** [where in the post]
- **License:** [Generated / CC BY / Unsplash Free / etc.]

## Placeholder coffee images (temporary ambiance slots,
unused in this post)

Carried over from the post-47 template. Not referenced
from this post's body. Safe to delete once the three
ambiance images for Post 61 are generated and installed.

- placeholder-coffee-01.jpg through -05.jpg: assorted
  Unsplash photos. See post-47's media README for
  individual attributions.

## Attribution Guidelines

- Always credit photographers and image generators.
- For generated images, log the model name, the date, and
  the prompt verbatim.
- For photographs, name the photographer (where known)
  and include a URL to the original.
- Include the licence; when using freely-licensed images,
  preserve attribution downstream.
