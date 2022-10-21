---
title: Documentation
reviewers:
---

## Introduction

The RCPCH Audit Engine / Epilepsy 12 documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/), which is a framework, separate from Django, which takes Markdown source files from `docs` and compiles them into a static HTML site. These static files are then served from our hosting resources.

## Setup Python and Pyenv

See LINK for a guide on how to set up a Pyenv virtual environment containing the correct version of Python.

The documentation repository contains a `.python-version` file which will automatically select the correct Pyenv for you when you navigate to the repository, as long as you have called your virtualenv `mkdocs`.

You need to have Material for MkDocs installed (this installs MkDocs as well for you)

In most circumstances this is simply `pip install mkdocs-material`, but if you hit issues then there is more information at <https://squidfunk.github.io/mkdocs-material/getting-started/>

## `mkdocs serve`

`mkdocs serve` starts up a development server which will auto-reload after changes to the source files, and will serve the documentation on [`localhost:8001`](http://localhost:8001).

## How to edit content

- Check out a **new local branch** on which to make the changes, with a **descriptive name**.
- Make changes to the Markdown files in the `docs` folder in the project root.
- Ensure any new or renamed files are listed in the `nav` element within `mkdocs.yml` or they won't show up.
- Save and the changes.
- The auto-reloaded site will show the changes.
- Commit the changes. Try to keep commits tidy and 'atomic' - in that ideally a single commit should be one new or edited piece of content, not a whole raft of changes. This allows us to easily select which commits to include.
- Push the changes and create a pull request to have them included in the main project.

## Reference guides

MkDocs and Material for MkDocs (the MkDocs theme we are using) have a host of features for making beautiful, practical, functional and easily navigable documentation.

### Markdown

Fundamental to the way the documentation works is the use of a simple set of text annotations called '[Markdown](https://daringfireball.net/projects/markdown/)', which are easily readable and editable as text files but can be compiled into HTML for web viewing. MarkDown is hugely popular across the web for rapid entry of web-native formatted text, being the basis of much of GitHub, StackOverflow, and Discourse's functionality.

Markdown uses characters like asterisks (`*`), hashes (`#`) and others, to effect its formatting. For example: `**bold**` to denote **bold** text. It's simple to get used to and, once you're used to it, very productive too. One advantage is that formatted text stays where it's been put, unlike with some word processors in which the GUI formatting tools can have you chansing formatting changes all over a document.

#### Online editing of Markdown

If you are new to Markdown editing, you can use GitHub's interface itself to edit online, by clicking the 'pencil' edit icon in the top right corner of any source code page. There are also external tools like [Prose.io](http://prose.io/) and [StackEdit](https://stackedit.io/) which give you a nice interface for editing MarkDown online, and will sync the changes with GitHub for you. If you need help getting set up, [contact us in the Signal chat](../contact/contact.md).

If Markdown seems daunting then another option is simply to edit the content in the word processor of your choice and then ask one of the RCPCH Incubator team to convert it to Markdown and add it to the documentation.

### Material for MkDocs

On top of the basic features of Markdown, MkDocs and the Material theme adds all the nice website appearance and many additional features for making beautiful documentation sites.

A good overview can be had from looking at the [Material for MkDocs Reference section](https://squidfunk.github.io/mkdocs-material/reference/) and from copying existing code in the documentation that does what you need.

### MkDocs

If you can't find functionality documented in the Material for MkDocs theme website, this is usually because it is functionality which comes from MkDocs, the underlying framework, itself. See the [MkDocs](https://www.mkdocs.org/user-guide/writing-your-docs/#writing-with-markdown) site for these features.

### Pymdownx extensions

Some of the features such as [Keys](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#keys) come from extensions like [Pymdownx](https://facelessuser.github.io/pymdown-extensions/extensions/arithmatex/)
