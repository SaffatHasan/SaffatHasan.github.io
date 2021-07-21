# Resume ![build](https://github.com/SaffatHasan/resume/actions/workflows/build.yml/badge.svg) ![style](https://github.com/SaffatHasan/resume/actions/workflows/pylint.yml/badge.svg)

This project contains the code to generate `Saffat Hasan`'s resume.

## Motivation

<div align="center">

![](https://imgs.xkcd.com/comics/is_it_worth_the_time.png)

</div>

### Why?

- I disliked writing Latex AND writing fancy summary bullets
- I had no (good) way to keep track of old resumes
- I fell into the sunken cost fallacy. I guess I got it working?

## What This Project Accomplishes

I've achieved a reasonable level of decoupling of data from formatting (data _structure_ is still coupled). You can see that there are two different formats:

- `templates/resume.tex`
- `templates/resume-simple.tex`

This project also leverages Github Actions to automatically generate the PDFs as build artifacts. The project automatically deploys the artifacts (resume PDFs) to the `gh-pages` branch of this repository as well as to [Drexel's student servers (tux)](https://www.cs.drexel.edu/~sh3292/resume.pdf).

## Folder Structure

- `templates` contains the template to be rendered
- `resources` contains my personal data
- `src` contains Python code that renders `templates` to `tex` files
- `Makefile` contains a single `run` target which generates resumes locally

### Credits

`templates/resume-simple.tex` Thanks to [@jakeryank](https://github.com/jakeryang/resume) and [@sb2nov](https://github.com/sb2nov/resume/)

`templates/resume.tex` Thanks to [@dnl-blkv](https://github.com/dnl-blkv/mcdowell-cv)
