# 😎 Group for apps and services on exascale research infrastructure (GASERI) website

The group is interested in scientific software development, high-performance computers, cloud computing, and the use of free open-source software in the development of applications and services for supercomputers and cloud platforms, specifically in the application of exascale computing to solve problems in computational biochemistry and related fields. Visit [the group website](https://group.miletic.net/en/) for more information.

## Prerequisites

Editing the website contents requires at least [the basic knowledge of writing Markdown in MkDocs](https://www.mkdocs.org/user-guide/writing-your-docs/).

## Obtaining the sources

Clone the repository using [Git](https://git-scm.com/):

``` shell
$ git clone https://github.com/gaseri/website.git
$ cd website
```

## Editing the contents

Make the edits you want using any text editor you like. Popular choices include [Visual Studio Code](https://code.visualstudio.com/), which supports [highlighting and previewing Markdown out of the box](https://code.visualstudio.com/docs/languages/markdown), [VSCodium](https://vscodium.com/), the community-driven and freely-licensed binary distribution of VS Code, [IntelliJ IDEA](https://www.jetbrains.com/idea/) with [the bundled Markdown plugin](https://www.jetbrains.com/help/idea/markdown.html), [Markdown Mode for GNU Emacs](https://www.emacswiki.org/emacs/MarkdownMode), and [Markdown Vim Mode](https://github.com/preservim/vim-markdown).

## Preparing the build environment

The website is built using [MkDocs](https://www.mkdocs.org/) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/). Make sure that you have [Python](https://www.python.org/) and [pip](https://pip.pypa.io/) installed on your system; these two packages can usually be obtained via the operating system's package manager (e.g. [APT](https://wiki.debian.org/Apt), [DNF](https://dnf.readthedocs.io/), [Pacman](https://wiki.archlinux.org/title/Pacman), [Zypper](https://en.opensuse.org/SDB:Zypper_usage), [FreeBSD pkg](https://docs.freebsd.org/en/books/handbook/ports/#pkgng-intro), [Homebrew](https://brew.sh/), or [Windows Package Manager](https://docs.microsoft.com/en-us/windows/package-manager/)).

Once Python and pip are successfully set up, start by installing the required Python packages using the `pip` command:

``` shell
$ pip install -r requirements.txt
```

## Previewing the website

To open a local web server that will serve the website contents for previewing, use the [MkDocs's serve command](https://www.mkdocs.org/getting-started/):

``` shell
$ mkdocs serve
```

## Building the website

Build the website using [MkDocs's build command](https://www.mkdocs.org/getting-started/#building-the-site) (any remains of the previous build will be cleaned up automatically):

``` shell
$ mkdocs build
```

If the build was unsuccessful, fix the errors and repeat the building process.

## Saving the edits

Once the build is successful, add the edited files using Git and commit the changes:

``` shell
$ git add docs
$ git commit
```

## Publishing the edits

To publish your edits in source form, push them to GitHub:

``` shell
$ git push
```

## Publishing the website

Once you have confirmed that the build is successful, push the built contents to GitHub using the [MkDocs gh-deloy command](https://www.mkdocs.org/user-guide/deploying-your-docs/):

``` shell
$ mkdocs gh-deploy
```

Wait a few minutes until [GitHub Pages](https://pages.github.com/) finishes building the new site from the changes you just pushed and then visit [group.miletic.net](https://group.miletic.net/) to make sure that your changes are visible.

*That's all, folks!*
