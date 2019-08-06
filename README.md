# jupyter-diagrams
Some diagrams relating to how Jupyter works, maybe?!

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ouseful-demos/jupyter-architecture-diagrams/master)


Diagrams are created using a variety of techniques:

- using image generators from [blockdiag.com/en/](http://blockdiag.com/en/);
- using the Draw.io editor (available via JupyterLab).

This repository also includes Jupytext, which allows notebooks to be created / edited as markdown files.

The diagrams are still very sketchy, and may not be true... What I'm trying to work towards is a set of simple diagrams that are quite easy to read, and give an overview of how the various pieces firt together,  and maybe some of the process steps taken by, a varety of Jupyter setups. They are not necessarily intended as documentation... If they're simplistic but not wrong, that's fine. If they are wrong, please let me know where...

## Working with Jupytext markdown

To create a new notebook, create a new text file in the `markdown` folder, with an `.md` suffix. Write your markdown with code contained in identified code blocks. For example:

`````
# Header

Some *markdown* text.

```python
#Some code...
print('hello')`
```


Did that work?
`````

Save and close the file, then click on it from the Jupyter file listing to launch it, under Jupytext, as a notebook.

A dual notebook is also saved in the hidden `.notebooks` directory.

## Working With *Draw.io* files

To open the *draw.io* application, open JupyterLab (replace the `\tree` path when launched from MyBinder, and click on the `Diagram` button in the *Launcher*.

Alternatively, from the JupyterLab file browser, in the `drawio` directory, double click on a `.dio` file to open it in *draw.io* within JupyterLab.

From draw.io [issues](https://github.com/jgraph/drawio/issues/384#issuecomment-518533528) / [docs](https://j2r2b.github.io/2019/08/06/drawio-cli.html):

> The drawio CLI also works with folders and the `-f` flag can be used to specify the format. To convert all the files in the files/ folder to png:
> ```
> $ mkdir out
> $ draw.io -x -f png -o out/ files/
> ```
> See [Draw.io from the command line](https://j2r2b.github.io/2019/08/06/drawio-cli.html) (In particular the "Convert multiple files" section at the end of the page)
