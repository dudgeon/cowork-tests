# Round 0: Just test the pattern

Starter template:
- basic COF generic template: [MLA Slide Template Empty.pptx](https://github.com/dudgeon/cowork-tests/blob/main/slides/test-01/MLA%20Slide%20Template%20Empty.pptx)

Prompt:
```
I want you to make a deck, using this as a template, to explain the core ideas in this blog post (https://wesmckinney.com/blog/mythical-agent-month/?utm_source=tldrnewsletter) -- use my chrome extension if you need to read it.

There are very few rules for our company's house style; but all titles are a complete thought or statement; use the 'blue boxes' slide to introduce big new ideas; and balance not oo much word density vs a deck that survives an offline read with no voice over--to do this you will need to get to the heart of the blog post and pull out its most important key take-aways, while making them feel real/tangible. Oh and very very little clipart; almost none.
```

Output:
- [mythical-agent-month.pptx](https://github.com/dudgeon/cowork-tests/blob/main/slides/test-01/mythical-agent-month.pptx)
- Proved the pattern (can roundtrip source Google Slides through Cowork via .PPTX files without breaking formatting; can extract key points into blue boxes, etc)
- Output lacked any kind of insight and took article at face value (arguably in line with the instruction)

## Enhance insight extraction and story telling

Instruction to Claude:
```
please research some best practices to extract insights from articles (not missing the forest for the trees; identifying the big "so what", expanding on topics that are intuitive to the source but may be a big insight to the reader) and constructing solid powerpoint/presentation narratives. then write an instruction that claude can understand and use to improve its synthesis and storytelling abilities
```

Output: [insight-synthesis-and-narrative-instruction.md](https://github.com/dudgeon/cowork-tests/blob/main/slides/test-01/insight-synthesis-and-narrative-instruction.md)

# Round 1: Test enhanced insight generation and narrative abilities

Continued from previous claude session (infer that starter deck is now [mythical-agent-month.pptx](https://github.com/dudgeon/cowork-tests/blob/main/slides/test-01/mythical-agent-month.pptx))

Prompt:
```
I would like you to try again; reread the new guidelines at the end of this prompt, reread the article, consider the guidelines, and make a v2 of your deck adhering to the guideline.

Guideline: {pasted [insight-synthesis-and-narrative-instruction.md]}
```

Output:
- [mythical-agent-month-v2.pptx](https://github.com/dudgeon/cowork-tests/blob/main/slides/test-01/mythical-agent-month-v2.pptx)
- First pass: much more insightful narrative
