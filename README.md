# Cognitive walkthrough
This Pandoc template may be used to generate sheets used in a Cognitive walkthrough, currently only in German.

As an example, the markdown file [example.md](example/example.md) with the content

```markdown
---
title: Beispiel 1
author: Christopher Gundler
actions:
- Nutzer drückt Button 1
- Nutzer klickt auf Textbox
- "Nutzer tippt: Die Antwort ist 42"
---

Das ist ein Beispiel für eine zu analysierende Aufgabe.
```
followed by the command 
`pandoc -s --template .\cognitive_walkthrough.latex -o example.latex .\example.md`
and the compilation of the resulting *example.latex* will result in [this example.pdf](example/example.pdf).
