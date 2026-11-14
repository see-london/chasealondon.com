# chasealondon.com

My personal site. The home page is one file, `index.html`, which holds all the content, styles and demos. The BTU calculator (`btu/`) and Pipeline Clicker (`pipeline/`) are their own pages. Fonts are self-hosted in `assets/fonts/`. It is hosted on Cloudflare Pages and redeploys automatically whenever this repo changes.

## Editing

1. Open `index.html` on GitHub and click the pencil icon.
2. Press Ctrl+F (Cmd+F on a Mac) to find the text you want to change, edit it, and click **Commit changes**.
3. The live site updates in about a minute.

## Where things live in index.html

| To change... | Search for |
|---|---|
| Colors (light and dark mode) | `:root{` at the top of the `<style>` block |
| Headline and intro | `class="hero"` |
| Fonts | `--ui` (Archivo) and `--body` (Source Serif 4) in the same `:root{` block |
| Career roles, bullets and tools | `const roles = [` (the timeline, detail panel and 60-second view all read from this) |
| How I work rows | `class="how"` |
| Project write-ups | `id="p-roi"`, `id="p-fin"`, `id="p-auto"`, `id="p-model"`, `id="p-loc"`, `id="p-call"`, `id="p-btu"`, `id="p-ab"` |
| Hero before-and-after cases | `const CASES = [` |
| Ideas section (T&F metrics, Levels of Automation) | `id="ideas"` |
| Tools timeline | `const TOOLS = {` |
| Off the clock hobby map | `id="off"` and `OFF THE CLOCK: HOBBY MAP` in the script |
| Contact details | `id="contact"` |
| The 60-second summary | `$('#skimSheet').innerHTML` |

## Tips

- Change a few things at a time. If something breaks, open the file's **History** on GitHub and restore the previous version.
- The timelines end at today's date automatically; there is no "now" value to update.
- After changing the headline, regenerate `assets/og.png` (the link-preview image) so it matches.
- To preview before publishing, download `index.html` and open it in your browser.

