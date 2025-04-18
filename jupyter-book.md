All recipes provided as markdown files are compiled into a Jupyter Book hosted under https://tillschwoerer.github.io/data-science-cookbook

Technically this requires the following steps:

1. Install the Jupyter Book package using pip:
```bash
pip install jupyter-book
```
2. Create a configuration file for the Jupyter Book. This file is typically named `_config.yml` and contains settings for the book, such as the title, author, and theme.

3. Create a structure for the book, dividing its contents into chapters and subchapters. This is defined in the file named `_toc.yml` (table of contents)

4. Write the content of the book in markdown files. Each recipe is a separate markdown file, and they are organized into folders according to the structure defined in `_toc.yml`.

5. Build the book using the command:
```bash
jupyter-book build .
```

This command generates the HTML files for the book in a folder named `_build/html`.

6. Optionally, you can preview the book locally using:
```bash
start _build/html/index.html    # Windows
open _build/html/index.html     # MacOS
```

7. Finally, we host the book on GitHub Pages or any other static site hosting service. For GitHub Pages, you can push the `_build/html` folder to the `gh-pages` branch of your repository. This can be done using the following commands:

```bash
git branch gh-pages
git switch gh-pages
git add _build/html     # once the book is built
git commit -m "Update Jupyter Book"
git push origin gh-pages
```