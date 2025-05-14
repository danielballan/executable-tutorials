# Executable Tutorials Repo setup best practices

## How to Run The Code Yourself

`````{tab-set}
````{tab-item} Locally with pixi

Clone the repository and launch JupyterLab.

```sh
git clone https://github.com/scientific-python/executable-tutorials
cd executable-tutorials

pixi run start
```
````

````{tab-item} Locally with pip

Clone the repository, create an enviornment, install the requirements, and
launch JupyterLab.


```sh
git clone https://github.com/scientific-python/executable-tutorials
cd executable-tutorials

python -m venv venv
source venv/bin/activate

pip install -r requirements.txt
jupyter lab
```
````

````{tab-item} In Cloud with Binder

[Open on Binder][].

````

````{tab-item} JupyterLite (experimental)

[Open with JupyterLite][].

````
`````

## Example Tutorials

```{toctree}
---
maxdepth: 1
glob:
caption: User tutorials
---

tutorials/**/*

```


## Contributing documentation

```{toctree}
---
maxdepth: 1
caption: Contributing
---

contributing
maintainer-guide
```

[Open on Binder]: https://mybinder.org/v2/gh/scientific-python/executable-tutorials/main?urlpath=tree/tutorials/
[Open with JupyterLite]: https://scientific-python.github.io/executable-tutorials/jupyterlite/lab/index.html
