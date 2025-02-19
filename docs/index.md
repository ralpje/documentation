# Welcome to MkDocs

Welcome to the ralpheckhard.com documentation library.
Pages are placesholders to showcase functionality that is available. 
For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Markdown

MKDocs uses Markdown for drafting documents. 

### Generic Markdown guide
A guide to using Markdown can be found [here](https://www.markdownguide.org/).

### MKDocs specific documentation
MKDocs uses the Python-Markdown processor, and you can enable additional extensions. Information on supported Markdown elements can be found [here](https://www.markdownguide.org/tools/mkdocs/#mkdocs-markdown-support).

### Material for MKDocs
Material for MKDocs is the theme used for this site. You can find references on the features available through this them [on the website](https://squidfunk.github.io/mkdocs-material/reference/).


## Project layout

The content of the site are defined by the file structure. The basic structure is depicted below. 

    mkdocs.yml                              # The configuration file.
    docs/
        index.md                            # The documentation homepage.
        Entra ID                            # Entra ID Directory, placeholder for all information
            Entra ID Connect                # Entra ID Connect Folder
                Various MD files            # Various MD files with information
            Introduction to Entra ID.md     # Basic info page on Entra ID

### Page ordering
In the various subfolders, there can be `.pages` file. This file will specify the orders in which pages are displayed in the navigation menu. 
For example:

```
nav:
 - Intro to Entra ID Connect.md
 - ...
 - Entra ID Connect.md
```

This code defines the first and last page and places other pages in between.
The `awesome-pages` plugin in used for this functionality, documentation can be found [on Github](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin?tab=readme-ov-file#features).
