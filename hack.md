---
title: Presentation Hacks
author: Michael Fudge
date: 8/21/2023
---

# Presentation Hacks!

Ween yourself off Powerpoint using Markdown, Pandoc and Reveal.js

by: Michael Fudge

---

## What's Wrong with Powerpoint ?

- Nothing!
- Powerpoint a great presentation tool with a lot of features.

![Relevant xkcd](https://imgs.xkcd.com/comics/scientific_paper_graph_quality.png)

---

## Downside of Powerpoint

- Cannot easily embed content from the web
- Does not support Bib/citations 
- UI "gets in the way; difficult to focus on the message"
- Proprietary: Not based on any standards

---

## Markdown, Pandoc, Reveal.js

- Markdown 
    - Lightweight language for formatting documents.
    - Easy to learn!
    - Text based
- Pandoc 
    - Convert documents to multiple formats
- Reveal.js
    - Build a slideshow from markdown
    - Pure HTML, runs in any browser!

---

## Here's how it works

[![](https://mermaid.ink/img/pako:eNqNksFOAjEQhl-lluvqBS80QkKARA0IATUhrIdxO3Ur3Za0syAhvLtddiEeTLSnmb_z_TPN9MAzJ5ELrozbZTl4YuN5alk8y-nLaulKcffue2wkNbGY-SqbeQxoCUg7yx5sJU3Ar6Xb2beanfWfhtPBagZWuqx2GDi7xWhPrkrnuEUwN5-B3T9Pxg01H72O-uPHxepyW6NDHTYG9r_2TyrB6DUyynVgzuJV43Z5Bet2e81Ep_DcJrV1SaC9wVOh0saIluqoJJB3axStdrvdxNc7LSkXt5uvn1RjW4Md9X_wPMS5p-r8ifKEF-gL0DLu61ApKaccC0y5iKFEBaWhlKf2GEuhJLfY24wL8iUmvNxIIBxq-PBQcKHAhKhi3Kvzk_oPnL7C8RtQdK6P?type=png)](https://mermaid.live/edit#pako:eNqNksFOAjEQhl-lluvqBS80QkKARA0IATUhrIdxO3Ur3Za0syAhvLtddiEeTLSnmb_z_TPN9MAzJ5ELrozbZTl4YuN5alk8y-nLaulKcffue2wkNbGY-SqbeQxoCUg7yx5sJU3Ar6Xb2beanfWfhtPBagZWuqx2GDi7xWhPrkrnuEUwN5-B3T9Pxg01H72O-uPHxepyW6NDHTYG9r_2TyrB6DUyynVgzuJV43Z5Bet2e81Ep_DcJrV1SaC9wVOh0saIluqoJJB3axStdrvdxNc7LSkXt5uvn1RjW4Md9X_wPMS5p-r8ifKEF-gL0DLu61ApKaccC0y5iKFEBaWhlKf2GEuhJLfY24wL8iUmvNxIIBxq-PBQcKHAhKhi3Kvzk_oPnL7C8RtQdK6P)

--- 

## More than just Reveal.Js

[![](https://mermaid.ink/img/pako:eNqdUl1LwzAU_SsxA5-mL_NlgQnDdqisa-mmIu0eQnNj49JkpKl1jP1307WrPs4FEm4O93xcuHucaQaYYC51neXUWDSPU4XceQ9fkoCaDdO1WrdQNF144UMSUcV01mGx_-pP58_LJIYvoPL2s0SPq2B-YnizxF00ExLWDdDB4ZsfR-HTYpVEugaz1ULZtqltCMLYT6aKoYCqHQq0gat1HwtNJvddlmN5ioCuG7_m7eXdp5FKVUsu7U7CUYILKcmAj_mwtEZvgAxGo1FX39SC2Zzcbb__sjrDljjm5xP7eJ0nH5_v6ca5gPU7_v_JF6TFQ1yAKahgbpH2DZJim0MBKSauZMBpJW2KU3VwrbSyerlTGSbWVDDE1ZZRC56gH4YWmHAqS4cCE1aboF3O444efgCODNkw?type=png)](https://mermaid.live/edit#pako:eNqdUl1LwzAU_SsxA5-mL_NlgQnDdqisa-mmIu0eQnNj49JkpKl1jP1307WrPs4FEm4O93xcuHucaQaYYC51neXUWDSPU4XceQ9fkoCaDdO1WrdQNF144UMSUcV01mGx_-pP58_LJIYvoPL2s0SPq2B-YnizxF00ExLWDdDB4ZsfR-HTYpVEugaz1ULZtqltCMLYT6aKoYCqHQq0gat1HwtNJvddlmN5ioCuG7_m7eXdp5FKVUsu7U7CUYILKcmAj_mwtEZvgAxGo1FX39SC2Zzcbb__sjrDljjm5xP7eJ0nH5_v6ca5gPU7_v_JF6TFQ1yAKahgbpH2DZJim0MBKSauZMBpJW2KU3VwrbSyerlTGSbWVDDE1ZZRC56gH4YWmHAqS4cCE1aboF3O444efgCODNkw)

---

##  Markdown

- Simple semantic method to format text.
- numbered and bulleted lists
- Supports images and links
- Code support
- Learn More: [https://commonmark.org/help/](https://pandoc.org/)

---

## Markdown Editors

- Any text editor will do.
- I use VS Code since it offers 
    - preview 
    - syntax help
    - spell check

---

## Pandoc

- The universal document converter
- Where can you get it?
- [https://pandoc.org/](https://pandoc.org/)

---

## Converting Markdown with Pandoc

- To Powerpoint: 
```bash
pandoc mymarkdown.md --output=mypowerpoint.pptx
```

---

## Converting Markdown with Pandoc

- To PDF: 
```bash
pandoc mymarkdown.md --output=mydocument.pdf
```

---

## Converting Markdown with Pandoc

- To Reveal.Js:
```bash
pandoc mymarkdown.md --output=mypresentation.html --to=revealjs 
   -s -V revealjs-url=https://unpkg.com/reveal.js/
```
- For the last one we nee to embed into a `-s` standalone file and 
- include the `revealjs-url` to load the presentation software

---

## Reveal JS

- Presentation in the browser. 
- Use Arrow keys
- Press `s` for speaker view
- Press `?` for help.

---

# What Can I do?

--- 

## IFrames / Embeds

<iframe width="560" height="315" src="https://www.youtube.com/embed/ySDX02WD0og" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---

## Math (MathJax)

When $$a \ne 0$$ there are two solutions to $$ax^2 + bx + c = 0$$ and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

---

## Code 

```Python
import pandas as pd
data = { 
    'name' : [ 'abby','bette','carl'],
    'age' : [ 40,34,50]        
}
df = pd.DataFrame(data)
```
---

## Tables

| Name | Age |
|-----|-----|
| abby | 40 |
| bette | 34 |
| carl | 50 |

---

## Embed Plots

<p align="center"><iframe width="100%" height="100%" style="border: 0px;min-height: 600px;" src="https://public.tableau.com/views/Regional_16766597857820/GlobalTemperatures?:showVizHome=no&:tabs=no"></iframe></p>

---

## Citing / Bib

- Don't breathe in the data exhaust [@zuboffBigOtherSurveillance2015].
- We love multidimensional social networks [@shumateEmergenceMultidimensionalSocial2013].

# Bibliography

Auto Generated From Your Citations!



