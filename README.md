# Pandoc Markdown Template

This template provides an easy way to write beautiful PDF's with Markdown.

## Requirements

1. Docker
2. VSCode, and the recommended Extensions (should popup when you open the workspace)

## How-to

### content/

Inside this folder is all the markdown files in your document. These are the files that will be compiled into your PDF.

If you only have one file you can call it whatever, and it will be picked up by the compiler.

If you want to split your document into multiple files, you have to know that they are compiled in the order they are listed in the files view. A good norm is to append the file with a number such as: "01-nameoffile" and "02-nameoffile", to ensure they are compiled in that order.

### filters/

Here you can add filters to pandoc, that enables more features. Take note that some filters requires external tools to exist. You can make a PR for the docker image (see https://github.com/niem94/docker.pandoc-plus) to include these, or request me to make the changes. If i do not approve of the tool, you can always clone my docker image and make your own.

### config/

In here is the configuration of the compiler. The default configuration is setup for an academic scene but you can check <https://pandoc.org/MANUAL.html> to see what other options you have availible.

- The `config.yml`file has the base configuration for pandoc.
- The `preamble.yml`file configures LaTeX, to allow glossaries and more. You can use this for multiple purposes, but i suggest creating another config file for other purposes.
- The `frontmatter.yml`is a basic configuration for a title page and abstract. In the default configuration this is not used, but instead a custom LaTeX title page has been added to support more advanced usages. To use this one instead uncomment the relevant line in `config.yml` (Remember to comment out the advanced page as well).

### resources/

All resources used in the document should be added here. LaTeX documents count as resources as well.
