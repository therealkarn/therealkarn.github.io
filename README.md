# therealkarn.github.io
MDS Portfolio

This is my personal website / blog that I built with Quarto. It has two computational posts, one in R and one in Python, that perform an analysis on penguin data. 

Please reach the site via: <https://therealkarn.github.io>

## Installation 

Install these first (this is what I used):

- Quarto 1.10.18
- R 4.6.1
- uv 0.12.5

uv will install python 3.14 and renv installs itself when R starts

## Website Build

In the terminal, run the following in order. Make sure that after the cd step, every code line is run from the top of the repo. 

- clone the repo and go to it

```bash
git clone https://github.com/therealkarn/therealkarn.github.io.git
cd therealkarn.github.io
```

- create the python enviro 

```bash
uv sync 
```

- get the r packages from renv

```bash
Rscript -e 'renv::restore(prompt = FALSE)'
```

- render the website

```bash
uv run quarto render
```

## Website View

The website is in the docs folder. You can open it with docs/index.html

- view the website

```bash
uv run quarto preview 
```

## The Data

The computational posts both use the Palmer Penguins dataset. It comes as a built in package in both R and Python; network will be needed to install the packages but not to render the website. 

[Palmer Penguins](https://allisonhorst.github.io/palmerpenguins/) dataset
(Palmer Station Antarctica LTER. Released under CC0).






