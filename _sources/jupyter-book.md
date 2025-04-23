# Jupyter Book

All recipes provided as markdown files are compiled into a Jupyter Book hosted under https://tillschwoerer.github.io/data-science-cookbook

If you are interested in how this is achieved, here are the steps:

1. Install the Jupyter Book package using pip:
```bash
pip install jupyter-book
```
2. Create a configuration file for the Jupyter Book. This file is typically named `_config.yml` and contains settings for the book, such as the title, author, and theme.
```bash
# _config.yml
title: "Data Science Cookbook"
author: "Cooking.py"
```

3. Create a structure for the book, dividing its contents into chapters and subchapters. This is defined in the file named `_toc.yml` (table of contents). Note that the file names need to be provided without the extension (.md)
```bash 
# _toc.yml
format: jb-book
root: intro
parts:
  - caption: Recipes
    chapters:
    - file: maultaschen
    - file: bananabread
    - file: ...
```

4. Write the content of the book in markdown files. Each recipe is a separate markdown file, and they are organized into folders according to the structure defined in `_toc.yml`.

5. Build the book . This command generates the HTML files for the book in a folder named `_build/html`. 

```bash
jupyter-book build .
```


6. Optionally, you can preview the book locally using:
```bash
start _build/html/index.html    # Windows
open _build/html/index.html     # MacOS
```

7. Finally, we push the `_build/html` folder to the `gh-pages` branch of our Github repository. 
```bash
pip install ghp                     # Install the package ghp once
ghp-import -n -p -f _build/html     # Execute for push to gh-pages
```

Note that in the settings of our Github repo, we have defined the location of the HTML files (Settings -> Pages -> Deploy from a branch -> gh-pages). Other alternatives are possible