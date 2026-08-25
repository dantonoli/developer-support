# PlainClip — Support

PlainClip is a menu bar utility for macOS that cleans the text you copy, so pasting stays plain
and predictable. It runs entirely on your Mac.

- **Requires:** macOS 14.0 or later
- **Privacy policy:** [PRIVACY/PlainClip.md](PRIVACY/PlainClip.md)
- **Ask a question or report a problem:** [Discussions](https://github.com/dantonoli/developer-support/discussions)

---

## Getting help

Open a post in [Discussions](https://github.com/dantonoli/developer-support/discussions) — that is
the fastest way to reach me, and answers stay visible for anyone with the same question.

| I want to… | Category to use |
|---|---|
| Report something broken | Q&A |
| Ask how a feature works | Q&A |
| Suggest a feature or a rule | Ideas |
| Show how you use it | Show and tell |

When reporting a problem, please include:

1. Your macOS version and PlainClip version (Preferences → About).
2. The app you copied **from** and the app you pasted **into**.
3. What you expected, and what you got instead.

A short before/after sample of the text helps most. Please remove anything private from it first —
never paste passwords, tokens, or personal data into a public post.

---

## What PlainClip does

Everything below is a separate switch in **Preferences → General**, so you can turn off anything
that does not suit your workflow.

**Formatting**

- **Auto-strip on copy** — rich copies become plain text.
- **Remove hidden characters** — strips invisible Unicode (zero-width spaces, soft hyphens, BOM)
  that web and chat copies often carry.
- **Remove hidden markers** — strips invisible marker characters (variation selectors, Unicode tag
  characters, direction controls) that some apps and tools embed in text.
- **Normalize smart quotes** — curly quotes and dashes become their plain equivalents.
- **Fix PDF line breaks** — rejoins lines broken by a PDF's column width.
- **Preserve list structure** — keeps bullet nesting when formatting is dropped.
- **Collapse blank lines** — removes runs of empty lines.

**Links**

- **Remove tracking parameters** — strips `utm_*` and similar, and unwraps AMP and redirect URLs
  back to the real destination.

**Traceability (off by default)**

- **Fingerprint copied text** — optionally embeds an invisible marker (copy time and an optional
  short label) into text you copy, so a paste can be traced back to the copy event. Off by default,
  manual only, and behind a confirmation dialog that explains the marker is detectable and readable
  by others. **Clean clipboard now** removes it.

**Exclusions**

- **Preferences → Exclusions** lets you name apps where PlainClip should leave the clipboard alone —
  useful for apps where formatting matters.

---

## Common questions

**PlainClip changed something I wanted to keep.**
Open the menu bar icon and choose **Pause PlainClip**, then copy again. To stop it permanently for
one app, add that app under **Preferences → Exclusions**. Individual rules can also be switched off
in **Preferences → General**.

**Can it tell me whether text was written by AI?**
No, and it does not claim to. **Check clipboard for hidden characters** reports invisible marker
characters only. Watermarks woven into the word choice of generated text cannot be detected or
removed by any character-level tool, PlainClip included. The app says so in its own results rather
than letting silence imply the text is unmarked.

**Does PlainClip send my clipboard anywhere?**
No. The app has no network entitlement and makes no network connections. There are no accounts, no
sign-in, and no analytics. Your clipboard is read and rewritten locally and never leaves your Mac.
See the [privacy policy](PRIVACY/PlainClip.md) for the full statement.

**Where are my settings stored?**
In your user preferences on this Mac. Removing the app removes its behaviour; nothing is left
running in the background.
