# Demo pkgdown website for bio3d v3.0

Quick and dirty test of possible pkgdown based bio3d website. See: < https://bioboot.github.io/web_demo/ >

## Requirements
Install the `pkgdown` and `tidytemplate` packages from CRAN.

Then we also need the following files in the bio3d package route directory (copies of these live in this repo under `SETUP_SITE/` dir - just copy these to the package root dir):
- _pkgdown.yml  
- index.md  
- logo.png
- FAQ.md  
- NEWS.md 

The main one here is the `_pkgdown.yml`   setting file (see example in `SETUP_SITE/` dir).

The rest are basically just regular old markdown text files that will be rendered to HTML by pkgdown `build_site()` function and used to comprise the website.

## Logo
The logo was made with the `hexSticker` package in the cwd:

```
library("hexSticker")

# Logo with text
sticker("tmp_logo1.png", package="bio3d",
			h_fill="white", h_color="#5484F5",
			p_color="#5484F5",
			p_y = 1.50, p_x = 1.01,
			p_family="Aller_Rg",
			p_size=10, s_x=1.01, s_y=.80, s_width=1,
			filename="logo_txt.png")

# Logo without text - i like this one best
sticker("tmp_logo1.png", package="",
			h_fill="white", h_color="#5484F5",
			p_color="#5484F5",
			p_y = 1.50, p_x = 1.01,
			p_family="Aller_Rg",
			p_size=10, s_x=0.99, s_y=0.99, s_width=1.15,
			filename="logo_notxt.png")
```

## Workflow
Use `build_site()` and `build_home()` from the **pkgdown** package to render and view site changes. The `lazy=TRUE` option is usefull whilst editing.

The vignettes require some special handeling, see below.

### Vignettes
The vignettes are annoying for a number of reasons - one is we don't include them in the package because they are too big (really this should be solved with a .build_ignore type mechanism). Another is they are in a separate "online" dir and we need to pass the path to each one relative to the vignettes dir to build_article/

Here is one way

```
build_article(name="online/pdb_vignette/Bio3D_pdb")
```

This places the output in the articles dir of the main website docs/ dir:

```
docs/articles/
```

> **N.B.** Note that the vignettes themselves were pulled from `git@bitbucket.org:Grantlab/bio3d-vignettes.git` and placed into the main `vignettes/online` dir of the bio3d package root dir. They need to be in a sub-dir of `vignettes/` here so as to not be included in the built package for CRAN etc.

**To Do:** setup a git sub-module for these vignettes...





