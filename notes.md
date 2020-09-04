# Creating presentations with jupyter notebook

Naming conventions:
* Call your notebook `presentation.ipynb`
* Name your html slides `index.html`

## Setup
1. Create a new virtual environment including `ipython` and `jupyter`

2. Install the RISE plugin to your environment with `pip install RISE` or `conda install -c conda-forge rise`

3. Add `reveal.js` as a submodule to your repository:
```
mkdir my-fancy-repo
cd my-fancy-repo
git init
git submodule add https://github.com/hakimel/reveal.js.git reveal.js
```

4. Create your presentation by launching `jupyter notebook`. From the menu select 'View' > 'Cell Toolbar' > 'Slideshow'. Now you can set the slide type for each notebook cell and make your presentation.

## Run your presentation with RISE

Simply click the enter/exit RISE slideshow button added to the right hand side of the jupyter notebook toolbar.

Navigating your RISE slideshow:
* SPACEBAR - Goes forward a slide in the slideshow
* SHIFT+SPACEBAR - Goes back a slide in the slideshow
* SHIFT+ENTER - Runs the cell on the current slide
* DOUBLE-CLICK - To edit a Markdown cell

### Alternative: serve slides as html
Here's how to serve your slides to a local https server (the code cells will be non-executable):

```
jupyter-nbconvert --to slides presentation.ipynb --post serve
```

## Download the slides as html and host on GitHub pages
From the jupyter notebook interface, click 'File' > 'Download As' > 'slides (.slides.html)'.

If you want to set up github pages to automatically point to this html file:

1. create a `docs/` directory in your repository,
2. Rename the file from `presentation.slides.html` to `index.html`
3. Put `index.html` in the root folder of the repository and commit it to git
4. In the settings of your repository, enable github pages from the root of the master branch

## Further reading
https://dzone.com/articles/creating-presentations-with-jupyter-notebook
