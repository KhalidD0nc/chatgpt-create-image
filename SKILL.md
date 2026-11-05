---
name: chatgpt-create-image
description: Route every image creation or image editing request to ChatGPT's image mode in the user's browser instead of generating images yourself or with any other model. Use for illustrations, photos, posters, covers, social visuals, logos in context, brand assets, and edits to existing images. Not for charts, diagrams, or UI mockups, which are better built in code.
---

# ChatGPT Create Image

ChatGPT has the strongest image model available to the user and generous limits on their subscription. So every image is made there. You prepare the brief, operate the browser, judge the result, and deliver it. ChatGPT makes the image.

## Scope

Use this for any raster visual: illustrations, photography-style images, posters, covers, thumbnails, social posts, brand visuals, and edits to existing images.

Do not use it for charts, data visualizations, diagrams, flowcharts, or UI screens. Those need exact numbers and text, so build them in code as usual.

## Workflow

1. **Gather what the image needs.** Find the relevant logos, brand colors, product photos, and past approved images on the user's computer, Drive, or the brand's website. Prefer original high-resolution files.
2. **Open ChatGPT in the browser** and start a new chat for each new image. Switch to image creation mode and confirm it is active. The UI changes over time, so act on intent, not exact labels.
3. **Attach references** and wait for uploads to finish.
4. **Send the brief** (see below).
5. **Review the result** against the brief: the logo, exact text, colors, and whether it serves its purpose.
6. **Refine in the same chat** when something needs fixing.
7. **Deliver**: download the image, save it where the task needs it, and show it to the user.

## Writing the brief

Brief ChatGPT the way you would brief a strong human designer. Split the brief into two layers:

- **Locked**: the purpose, the audience, the aspect ratio, exact visible text, brand colors, and the attached logo to be used as-is. State these clearly.
- **Open**: composition, visual metaphor, lighting, and style. Describe the feeling you want, then leave the visual decisions to ChatGPT. Do not dictate layouts in detail; ChatGPT's visual judgment is better than a prescriptive description.

Match freedom to the stage:

- **Exploring** a new idea: keep it loose. Ask for several distinct directions in one image as a concept sheet, then pick one.
- **Refining**: say what to keep and what to change ("keep the composition and colors, make the background calmer") so good parts don't drift.
- **Finalizing**: lock everything approved and only adjust sizes or variants.

If results come out generic, strengthen the concept and feeling, not the execution details. If they come out off-brand, tighten the locked layer or attach a past approved image as a style reference.

## The one rule

Never create or modify the image yourself: no native image tool, no other model, no SVG, Canvas, Pillow, or HTML rendering. Every change, including text corrections and color fixes, goes back to ChatGPT. If ChatGPT is unreachable, tell the user what is blocking and stop.
