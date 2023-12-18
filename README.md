# Markdown-Resume-Generator

Markdown resume generator using GitHub actions to output DOCX and PDF versions of your resume.

## Example Front YAML

```yaml
fontsize: 12pt
geometry: "left=1in,right=1in,top=1in,bottom=1in"
title: Curriculum Vitae
author: John Smith
subtitle: Penetration Tester & Security Researcher
preamble: I enjoy tinkering with computers...
```

## Usage

1. Clone this template repository
2. Make changes to the YML and MD files
3. GitHub action automatically runs on changes
4. Downoad the ZIP file by navigating to Actions -> Summary -> Artifacts -> resume

## Example Output

### PDF

![Screenshot of Markdown to PDF resume](resume.png?raw=true "Screenshot of Markdown to PDF resume")

### DOCX

![Screenshot of Markdown to DOCX resume](resume-docx.png?raw=true "Screenshot of Markdown to DOCX resume")

## Docker Usage

If you prefer not to use GitHub actions you can also run this locally with Docker. You can do this with Docker as `docker run --rm --volume "`pwd`:/data" --user `id -u`:`id -g` pandoc/latex resume.md -H header.tex --output=resume.pdf`.

# Resources

1. [Pandoc Docker files](https://github.com/pandoc/dockerfiles)
