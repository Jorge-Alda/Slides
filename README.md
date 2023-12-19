# Slides

Collections of slides for all my public presentations starting on 2022

## Index of slides

### 2022

* Unizar Seminar, 2022-01-20: [Branch](https://github.com/Jorge-Alda/Slides/tree/Unizar202201), [Slides](https://github.com/Jorge-Alda/Slides/releases?q=tag:002).
* IFT Seminar, 2022-01-27: [Branch](https://github.com/Jorge-Alda/Slides/tree/IFT2022), [Slides](https://github.com/Jorge-Alda/Slides/releases?q=tag:001).
* XIII CPAN Days, 2022-03-22 [Branch](https://github.com/Jorge-Alda/Slides/tree/CPAN22), [Slides](https://github.com/Jorge-Alda/Slides/releases?q=tag:003).
* Thesis Defense, 2022-04-27: [Branch](https://github.com/Jorge-Alda/Slides/tree/thesisdef), [Slides](https://github.com/Jorge-Alda/Slides/releases?q=tag:004).
* 5th Inter-experiment Machine Learning Workshop, 2022-05-09: [Branch](https://github.com/Jorge-Alda/Slides/tree/CERN22), [Slides](https://github.com/Jorge-Alda/Slides/releases?q=tag:005).
* Saturnalia 2022, 2022-12: [Branch](https://github.com/Jorge-Alda/Slides/tree/Saturnalia2022), [Slides](https://github.com/Jorge-Alda/Slides/releases?q=tag:006).

### 2023

* Saturnalia 2023, 2023-12-20: [Branch](https://github.com/Jorge-Alda/Slides/tree/Saturnalia2023), [Slides](https://github.com/Jorge-Alda/Slides/releases?q=tag:007).

## How does this repo work?

This branch (`main`) contains beamer templates and institutional logos. The slides for each event are in their own branch. When a new tag is pushed in a branch, GitHub Actions compiles the beamer files and produces a PDF [IMPORTANT: tags have to be pushed from the command line with `git push --tags`, creating a tag from GitHub's web won't work]. A tag version, like [`001.211218.01`](https://github.com/Jorge-Alda/Test/tree/001.211218.01), is formed of three parts:

* `slides id`: unique identifier for each event, a number starting on `001`.
* `timestamp`: date of the tag, output from `date "+%y%m%d"`.
* `tag id`: in case there are multiple tags the same day.

The file `README.md` of the branch is used as release notes.

GitHub Actions compiles by default the document `slides.tex`. To compile documents with another name, change the variable `env.MAIN_FILE`.

To include the tag in the PDF file (for example, for a perma-link), include the string `++TAGNUM++` in all `.tex`files.
