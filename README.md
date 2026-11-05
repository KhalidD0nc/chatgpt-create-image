# chatgpt-create-image

A Claude skill that hands every image job to ChatGPT's image mode in your browser. Claude writes the brief, drives the browser, judges the result, and delivers the file. ChatGPT makes the pixels.

## Why

If you already pay for ChatGPT, its image model is likely the best one you have access to, and your subscription limits are generous. Claude is better at the parts around the image: gathering brand assets, writing a sharp brief, checking the output against requirements, and putting the file where it belongs. This skill splits the work along that line.

## What it covers

**Use it for** raster visuals: illustrations, photo-style images, posters, covers, thumbnails, social posts, brand visuals, and edits to existing images.

**Don't use it for** charts, data visualizations, diagrams, flowcharts, or UI mockups. Those need exact numbers and text, so Claude builds them in code as usual.

## How it works

1. **Gather** logos, brand colors, product photos, and past approved images (prefer original, high-res files).
2. **Open ChatGPT** in the browser, start a new chat per image, and switch to image mode.
3. **Attach references** and wait for uploads to finish.
4. **Send the brief.**
5. **Review** the result against the brief: logo, exact text, colors, fit for purpose.
6. **Refine** in the same chat.
7. **Deliver**: download, save where the task needs it, show the user.

### The brief has two layers

| Layer | Contains | How to write it |
|---|---|---|
| **Locked** | Purpose, audience, aspect ratio, exact visible text, brand colors, attached logo used as-is | State plainly. Non-negotiable. |
| **Open** | Composition, metaphor, lighting, style | Describe the feeling; let ChatGPT decide the visuals. |

Freedom shrinks as the work matures: loose concept sheets when **exploring**, "keep X, change Y" when **refining**, everything locked except sizes and variants when **finalizing**.

Generic results → strengthen the concept and feeling. Off-brand results → tighten the locked layer or attach an approved image as a style reference.

### The one rule

Claude never creates or edits the image itself: no native image tool, no other model, no SVG, Canvas, Pillow, or HTML rendering. Every change, including text and color fixes, goes back to ChatGPT. If ChatGPT is unreachable, Claude says what's blocking and stops.

## Requirements

- A ChatGPT account with image generation, signed in in your browser.
- A Claude setup that can drive that browser, such as [Claude in Chrome](https://claude.ai/chrome) or the built-in browser in the Claude desktop app.

## Install

**Claude apps (claude.ai / desktop):** zip the folder containing `SKILL.md` and upload it as a custom skill in Claude's settings ([how-to](https://support.claude.com/en/articles/12512180-using-skills-in-claude)).

**Claude Code:**

```bash
git clone https://github.com/KhalidD0nc/chatgpt-create-image ~/.claude/skills/chatgpt-create-image
```

Then just ask for an image ("make a cover for my blog post on RAG"). The skill's description tells Claude when to use it.

## Notes

- Anything you attach as a reference is uploaded to ChatGPT. Don't attach confidential assets you wouldn't share with OpenAI.
- ChatGPT's UI changes often, so the skill tells Claude to act on intent rather than exact button labels.

## License

[MIT](LICENSE)
