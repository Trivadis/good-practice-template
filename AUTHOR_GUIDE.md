# Author and Release Guide

## Document Structure

### Folders

### Markdown Files

### Document Metadata

Pandoc document conversion can be configured / customized using metadata either
as a metadata block in the Markdown file itself or in a dedicated
[YAML](https://yaml.org/spec/1.2/spec.html) file. See also the
[pandoc documentation](https://pandoc.org/MANUAL.html). The workflow in this
repository is configured to use a dedicated metafile for each language. The file
is named `metadata.yml` and located in the corresponding directory (e.g.
[en/metadata.yml](en/metadata.yml) or [de/metadata.yml](de/metadata.yml))

It is strongly recommended to adjust the metadata according to the requirement
of the respective *good practice*.

## Good Practice Rules

### Numbering

### Mandatory Information

## Additional Language

## Create a Release

## Creating a new *Good Practice* Guide

## Build Documentation

### Automatic Build Workflow

### Manual Build

#### Docker Container

Creating the documents with the help of pandoc container
[oehrlis/pandoc](https://github.com/oehrlis/pandoc_template) is the most
convenient method. Apart from having Docker installed, there are no other
dependencies. The container xxx contains all the necessary components like
pandoc, TeX, fonts, templates, etc.

- Generate a PDF document

```bash
docker  run --rm -v "$PWD":/workdir:z oehrlis/pandoc \
--metadata-file=en/metadata.yml \
--pdf-engine=xelatex \
--resource-path=images \
--output=tvd-good-practice-template_en.pdf en/?x??-*.md
```

- Generate a DOCX document

```bash
docker  run --rm -v "$PWD":/workdir:z oehrlis/pandoc \
--metadata-file=en/metadata.yml \
--resource-path=images \
--output=tvd-good-practice-template_en.docx en/?x??-*.md
```

#### Local pandoc Installation

If you do have a local *pandoc* installation including LaTeX, you may also
generate the corresponding documents directly using `pandoc` via command line.
But be aware of the necessary requirements. e.g. fonts, LaTeX, etc.

- Generate a PDF document

```bash
pandoc --metadata-file=en/metadata.yml \
--template=$(pwd)/templates/trivadis.tex \
--pdf-engine=xelatex \
--resource-path=images \
--output=tvd-good-practice-template_en.pdf en/?x??-*.md
```

- Generate a DOCX document

```bash
pandoc --metadata-file=en/metadata.yml \
--reference-doc templates/trivadis.docx \
--resource-path=images \
--output=tvd-good-practice-template_en.docx en/?x??-*.md
```

- Generate a standalone HTML document

```bash
pandoc --metadata-file=en/metadata.yml \
-s --toc --template=$(pwd)/templates/GitHub.html5 \
--resource-path=images \
--output=tvd-good-practice-template_en.html en/?x??-*.md
```

- Generate a EPUB document

```bash
pandoc --metadata-file=en/metadata.yml \
--reference-doc templates/trivadis.epub \
--resource-path=images \
--output=tvd-good-practice-template_en.epub en/?x??-*.md
```
