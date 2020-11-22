# Pandoc Markdown Template

This template provides an easy way to write beautiful documents with Markdown.

## Requirements

1. Install LaTeX
2. Install pandoc
3. Install VSCode
   1. Install my Markdown Extension Pack from the VSCode Extension store -> "niem94.markdown-extension-pack"
   2. Open the workspace for a repository created from the template.
4. Write your document!

## Suggestions if VSCode is used

You can preview the section you are writing by using the command "Pandoc Markdown Preview".

## Building the full report

To build the document write "pandoc -o mydocument.pdf content/*.md" in the terminal, or run the included task "pandoc build"

There is currently no smart way to build the full report for the pandoc preview or compiler extension.