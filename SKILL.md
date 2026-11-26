---
name: 文献引用
description: Use when the user pastes work titles, a draft bibliography, or citation queries and wants entries checked against authoritative catalogs, then formatted as a copy-pasteable English reference list—especially for mixed Chinese primary sources, modern Chinese scholarship, and Western theory.
---

# 文献引用

When the user gives work titles, raw citations, or a reference list, verify the bibliographic data and return a finished, copy-pasteable English reference list. Follow the typography, name, and translation rules below unless the user or a venue stylesheet overrides them.

## Style

- Default: Chicago notes-bibliography. The year belongs at the end of the publication facts, not immediately after the author.
- If the user names APA, author-date, a conference template, or pastes a sample, follow that instead. Do not assume a society-specific stylesheet.
- Drop Chinese document-type tags such as `[M]` and `[J]`. Do not keep the user’s original numbering unless they ask for a numbered list.
- In References, list the work as a whole. Put `juan`, chapter, and page numbers in notes or in-text citations, not inside the book title. Distinguish premodern `juan` from modern `vols.`

## Workflow

1. Inventory the items. Deduplicate the same work listed twice (for example a primary text plus its modern edition). Cite the edition the user actually used.
2. Verify metadata, unless the user says the sources are already checked.
   - Chinese premodern texts: confirm author or compiler, modern editor or punctuator, edition, volume count, place, publisher, and year from library catalogs or the publisher. Treat repositories such as 识典古籍, ctext, or Wikisource as finding aids; cite the edition actually consulted.
   - Modern Chinese books and articles: confirm author, title, journal, volume, issue, year, and pages from the official journal page, a library catalog, or the PDF first page.
   - Western books and articles: confirm from the publisher page, library catalog, or DOI. Use the translator, imprint, and year of the edition cited.
   - Never invent years, pages, ISBNs, DOIs, or edition statements. Omit or briefly flag what cannot be confirmed.
3. If the user says the bibliography is already verified, use their data and deliver a finished list with no verification markers, caveats, or source-criticism notes.
4. Format every entry with the typography and translation rules below, then arrange and deliver the list.

## Typography

- Book and journal titles are italic. Include the original Chinese in the same italic span, e.g. `*Taiping guangji 太平广记*`.
- Article and chapter titles are not italic. Use romanized title in quotation marks, then the Chinese title: `"Yulunpao zhuan" 郁轮袍传`.
- Keep simplified or traditional Chinese as given by the user or the source. Do not convert scripts.
- Pinyin is unmarked (no tone marks) unless the venue requires tones.

## Translation and names

- Do not add a bracketed English gloss or invented translation of a Chinese title.
- If the user is citing a published translation, use that edition’s official title, translator, and publication facts.
- Individual authors, editors, collators, and commentators of Chinese-language works: romanization plus Chinese characters, e.g. `Xia Hanyi 夏含夷`, `Li, Fang 李昉`.
- Institutional or corporate authors may stay in romanization only, e.g. `Shanghai guji chubanshe, ed.`
- Western authors of English-language works: no Chinese characters.

## Entry shapes (Chicago notes-bibliography)

Book:

`Author, Given 汉字. *Romanized title 中文题名*. Edited / punctuated / translated by Name 汉字. x vols. Place: Publisher, year.`

Journal article:

`Author, Given 汉字. "Romanized article title" 中文篇名. *Romanized journal 中文刊名* vol, no. x (year): pages.`

## Arrangement

When the paper mixes original texts, historical or literary studies, and theory, group the list as:

- **Primary Sources and Editions** — original texts and modern critical or punctuated editions
- **Historical and Literary Scholarship** — modern monographs and articles about the sources
- **Theoretical Works** — theoretical works in any language

Sort each group alphabetically by romanized author name. If the venue requires one alphabetical References list, merge the groups.

## Delivery

- Return a finished markdown list so italics are marked with `*...*`.
- If the user needs to paste into Word, offer or provide a `.docx` that uses italic character style, not asterisks.
- Lead with the list. Mention a correction only when it changes what the user thinks they cited (for example a different edition than the one they named).
- If the user later supplies a venue template, restyle the same data to that template; do not re-litigate verified facts.
