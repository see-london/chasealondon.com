# chasealondon.com

My personal site. It's one file, `index.html`, which holds all the content, styles and demos. It is hosted on Cloudflare Pages and redeploys automatically whenever this repo changes.

## Editing

1. Open `index.html` on GitHub and click the pencil icon.
2. Press Ctrl+F (Cmd+F on a Mac) to find the text you want to change, edit it, and click **Commit changes**.
3. The live site updates in about a minute.

## Where things live in index.html

| To change... | Search for |
|---|---|
| Colors (light and dark mode) | `:root{` at the top of the `<style>` block |
| Headline and intro | `class="hero"` |
| The three stat boxes | `class="stats"` |
| Career roles, bullets and tools | `const roles = [` (the timeline, detail panel and 60-second view all read from this) |
| Project write-ups | `id="p-model"`, `id="p-loc"`, `id="p-btu"`, `id="p-ab"` |
| Skills and their groups | `const groups = {` |
| Off the clock cards | `id="off"` |
| Contact details | `id="contact"` |
| The 60-second summary | `$('#skimSheet').innerHTML` |

## Tips

- Change a few things at a time. If something breaks, open the file's **History** on GitHub and restore the previous version.
- A tool name in a role's `tools` list must match the name in `groups` exactly, or the skill highlighting won't find it.
- To preview before publishing, download `index.html` and open it in your browser.

