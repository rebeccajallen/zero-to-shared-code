# Zero to Shared Code

A setup walkthrough that takes complete beginners from an empty laptop to a GitHub
link they can share. Six parts, a Windows/Mac toggle, and a checkpoint after every
step so nobody has to guess whether it worked.

Written for K–12 teachers learning to teach computer science, but it assumes nothing
beyond being able to download a file.

**Live site:** https://rebeccajallen.github.io/zero-to-shared-code/

---

## What's in here

| File | What it is |
|---|---|
| `index.html` | The whole guide. One self-contained file — all styling and scripts are inside it. |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is instead of running them through a blog engine. |
| `README.md` | This file. GitHub shows it on the repository's front page. |
| `LICENSE` | Terms for reuse. See the note at the bottom. |

There is no build step, no framework and nothing to install. Open `index.html` in a
browser and it works, online or off.

---

## Publishing it to GitHub Pages

GitHub Pages turns a repository into a real website for free. Once it's on, every
push you make updates the live page within a minute or two.

1. Push this folder to a GitHub repository (Parts 4 and 5 of the guide cover how).
2. On the repository page, click **Settings**.
3. In the left sidebar, under *Code and automation*, click **Pages**.
4. Under *Build and deployment* → *Source*, choose **Deploy from a branch**.
5. Set the branch to **main** and the folder to **/ (root)**, then click **Save**.
6. Wait. The first publish takes a few minutes; later ones are faster. Refresh the
   Pages settings screen and it will show you the address when it's live.

Your site will be at:

```
https://YOUR-USERNAME.github.io/REPOSITORY-NAME/
```

So a user called `jsmith` with a repository called `zero-to-shared-code` gets
`https://jsmith.github.io/zero-to-shared-code/`.

### One catch worth knowing before you start

**On a free GitHub account, Pages only works on _public_ repositories.** If you keep
this repository private, the Settings → Pages screen will tell you the feature isn't
available. Paid plans (Pro, Team, Enterprise) can publish from private repositories.

This is a useful thing to explain to a class, because it's the first time the
public/private choice from Part 6 has a visible consequence.

---

## Editing it

Everything lives in `index.html`. It's plain HTML with a `<style>` block at the top
and a small `<script>` at the bottom — no build tools.

Things you might reasonably want to change:

- **Times and part order.** Search for `part-min` to find the minute estimates, and
  the table of contents near the top of the `<body>`.
- **Your own institution's notes.** Each part is a `<section class="part">`, so you
  can add one by copying the shape of an existing section.
- **The colors.** All of them are defined once as custom properties in the `:root`
  block at the top of the `<style>` section, with a matching dark-mode set below it.
  Change them in those two places and the whole page follows.
- **Screenshots.** The guide uses drawn diagrams rather than captured screenshots so
  they work in dark mode and stay sharp. If you'd rather use real screenshots, drop
  the images in an `images/` folder and swap them in.

The page prints well, too — `Ctrl/Cmd + P` produces a clean handout with both the
Windows and Mac instructions shown and every collapsible section expanded.

---

## Credits

Two videos are linked from the guide at the points where they're most useful:

- *How to Connect GitHub to Visual Studio Code* — Saad Qureshi Official
- *How To Share a Link To a GitHub Repository*

Steps and menu names reflect versions current as of September 2026. VS Code updates
monthly, so a button occasionally moves.

---

## License

This guide is released under [Creative Commons Attribution 4.0
International](https://creativecommons.org/licenses/by/4.0/) — anyone may share and
adapt it, including commercially, as long as they credit the original.

**This was a default choice, not an instruction.** CC BY is the usual pick for open
educational resources, but if your institution has a policy or you'd rather use
something else, replace the `LICENSE` file and this section. If you don't want to
license it for reuse at all, delete both — though note that a public repository with
no license still lets people view and fork it.
