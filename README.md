# Plain English Summarization of Contracts


Please cite our [NAACL NLLP Workshop paper](https://www.aclweb.org/anthology/events/ws-2019/#w19-22) as:

```
@inproceedings{manor-li-2019-plain,
    title = "Plain {E}nglish Summarization of Contracts",
    author = "Manor, Laura  and
      Li, Junyi Jessy",
    booktitle = "Proceedings of the Natural Legal Language Processing Workshop 2019",
    month = jun,
    year = "2019",
    address = "Minneapolis, Minnesota",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/W19-2201",
    pages = "1--11",
}
```

## Files
* all_v1.json: 446 sets from both websites
* tldrlegal_v1.json: 84 sets from [https://tldrlegal.com](https://tldrlegal.com)
* tosdr_annotated_v1.json: 84 sets from [https://tosdr.org/](https://tosdr.org/)

## Data
This dataset consists of the data included in the quantitative analysis as described in the paper. Sets which had a reference summary with more tokens than the original text are excluded.
Each set consists of: 
* uid: unique identification string
* original_text: cleaned & parsed original text
* reference_summary: cleaned & parsed reference summary
* doc: name of the document which the original text is from
### TL;DRLegal
Each tldrlegal set may also have: 
* title: "title" of the set (from website)
### TOS;DR
Each tos;dr set may also have:
* note: Mostly empty, a space for additional notes from the annotator
* urls: URL of the respective company
* case_text: raw text from the "case" (from website)
* case_code: annotation for "case" text 
* title_text: raw text from the "title" (from website)
* title_code: annotation for "title" text 
* tldr_text: raw text from the "tldr" (from website)
* tldr_code: annotation for "tldr" 

A note on annotation: 
* Each code begins with a number, which is the 'ranking' of the quality of the respective text as chosen by the annotator
* A code may also have a letter, which stands for:
  * s: standard -- this exact text (without company names) occurs at least one other time in a different set. 
  * j: jurisdication -- this text deals with jurisdiction
  * q-: quote(-) -- this text is excerpt of the original text
  * d: description -- this text is a description of what the original text talks about, but may not give details




