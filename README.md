# PsycheDive

> A quiet corner for the questions that keep circling in your head.

Type a feeling, a situation, or a concept. PsycheDive reads real psychology research (**Europe PMC** + **OpenAlex**) and writes an evidence-checked explanation. Then it helps you keep what you learned with bookmarks, a concept map, games and PDF export.

![Version](https://img.shields.io/badge/version-B%20%C2%B7%20Field%20Notebook-2B6173)
![Single file](https://img.shields.io/badge/app-single%20HTML%20file-5EACB2)
![No install](https://img.shields.io/badge/install-none-4E75AB)
![Dark mode](https://img.shields.io/badge/dark%20mode-teal%20palette-9CB6C2)

> **Educational psychology only.** PsycheDive is not a diagnostic or therapy tool. If something feels heavy, please talk to a qualified professional or someone you trust.

---

## What's in this repository

| File | What it is |
|---|---|
| `psychedive.html` | The whole app: design, logic and content in one file. No build step, no server, no dependencies to install. |
| `README.md` | This guide. |

---

## Quick start

1. Download `psychedive.html`.
2. Double-click it to open it in your browser (Chrome, Edge, Firefox or Safari).
3. Open **Settings → Groq API key** and paste your free key from <https://console.groq.com/keys>.
4. Type something you've been wondering about.

That's it. You need an internet connection, because the research sources, the AI model and the fonts all load online.

### Optional: web search

For extra web results, add a Tavily key in **Settings** (it starts with `tvly-`). Get one at <https://app.tavily.com/home>. The app works without it.

### Optional: put it online with GitHub Pages

1. In your repository go to **Settings → Pages**.
2. Under *Build and deployment*, choose **Deploy from a branch**, pick your main branch and the `/ (root)` folder, then save.
3. After a minute the app is live at `https://<your-username>.github.io/<repo-name>/psychedive.html`.

Each visitor pastes their **own** key in Settings. Your key is never part of the site.

---

## Features

| # | Feature | Where it lives |
|---|---------|----------------|
| 1 | **Home button**: jump back to the desk from anywhere | floating 🏠 button, top-left, also in Settings |
| 2 | **Text size**: bigger or smaller, remembered on the device | `A−  100%  A+` control, top-left, also in Settings |
| 3 | **Concept bookmarks**: save the ideas you like and reopen them | ☆ Bookmark in every read, 🔖 panel, homepage section |
| 4 | **No-repeat game questions**: cases never come back until the set runs out | automatic in all case/scenario games |
| 5 | **Export as PDF**: turn a finished read into a document | button on each finished read |
| 6 | **Dark mode**: easier on the eyes at night | Settings → Dark mode |

---

## Version B: "Field Notebook"

Version B is a visual restyle. Same app, same content, new look.

- **Type:** *Baloo 2* for headings, *Mukta* for reading text, *Kalam* for handwritten annotations.
- **Notebook feel:** ruled paper on the left page, graph paper on the right, masking tape, highlighter strokes and soft paper shadows.
- **Dark mode ("teal palette"):** a deep teal-navy desk with mist-blue headings and a warm taupe accent. It keeps both the ruled page and the graph page.
- **Reading font choices in Settings:** *Note hand*, *Reading text* and *Rounded*.
- **PDF export** uses the same fonts, and the text-size control works everywhere.

### Dark palette

| Swatch | Hex | Used for |
|:--:|:--:|---|
| ![#2B6173](https://img.shields.io/badge/-%20%20%20-2B6173) | `#2B6173` | deep teal: page tape, base of the dark surfaces |
| ![#5EACB2](https://img.shields.io/badge/-%20%20%20-5EACB2) | `#5EACB2` | teal: correct answers, borders, mapped concepts |
| ![#9CB6C2](https://img.shields.io/badge/-%20%20%20-9CB6C2) | `#9CB6C2` | mist: headings, links, secondary text |
| ![#4E75AB](https://img.shields.io/badge/-%20%20%20-4E75AB) | `#4E75AB` | sea blue: text selection |
| ![#B39F95](https://img.shields.io/badge/-%20%20%20-B39F95) | `#B39F95` | taupe: sticky notes, margin line, warm accents |

---

## Privacy and data

- **Everything you save stays in your browser**, in local storage on your device. There is no PsycheDive account or server.
- Your Groq key (and Tavily key, if you add one) is stored **only in that browser**. It is not in `psychedive.html` and not in this repository.
- Stored locally: your concept library, bookmarks, text size, game progress, display settings (such as dark mode) and your keys.
- To answer a question the app sends your text to the services it uses: **Groq** (writes the explanation), **Tavily** (optional web search), **Europe PMC** and **OpenAlex** (research papers). It also queries Wikipedia and the Internet Archive. Don't type anything you wouldn't want sent to those services.
- Clearing your browser's site data erases your library, bookmarks and keys. Use a private/shared computer with care: remove your key in Settings when you're done.

---

## Troubleshooting

| Problem | Try this |
|---|---|
| The page looks plain, with default fonts | The fonts load from Google Fonts. Check your internet connection and reload. |
| The "add your Groq key" note keeps showing | Paste the key in **Settings → Groq API key**, then try again. |
| Explanations never appear | Confirm the key is valid at <https://console.groq.com/keys> and that you're online. |
| Dark mode isn't on | Open Settings and switch **Dark mode** on. It is remembered per browser. |
| Text is too small or too large | Use `A−` / `A+` at the top-left. It shows `100%` at the default size. |
| My bookmarks are gone | They live in one browser on one device. A different browser or cleared site data starts fresh. |

---

## Notes

- Educational psychology only. It is not a diagnostic or therapy tool.
- The games are illustrations of how psychological reasoning works. A single behaviour never identifies a person.
- Research summaries are generated by an AI model from the sources it finds. Check the cited papers before relying on anything.
