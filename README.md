# Capstone-Skynet.github.io
This repository contains the documents and notes

**This repository is for notes, posts, documentations, and other archives.**

## How To Start Modifying this Repo

First clone this repository into your local drive.

```shell
git clone https://github.com/Capstone-Skynet/Capstone-Skynet.github.io.git
``` 

or if you're using SSH:

```shell
git clone git@github.com:Capstone-Skynet/Capstone-Skynet.github.io.git
```

Then you can modify its contents.

- All the weekly meeting agendas and notes are located under *_notes* folder.
- All the updates and WSR's are located under *_posts* folder.


## Adding Notes

To add notes, create a new `.md` file under *_notes* folder and the name should follow the pattern: "YYYY-mm-dd-title.md".
The the very top of the .md file, add the following *front matter* metadata so that the static website generator can
categorize and sort it:

```gfm
---
date: 2019-09-16
title: "Your title"
author: "Your name(s)"
---
```

### Adding Images and Other References

Please ensure that all references to images are either **relative** or online (using URL).

## Adding posts

Posts are more like weekly status reports (WSRs) and project progress updates. To add posts, create a new `.md` file under *_posts* and
follow the same steps for notes. Make sure to copy and modify the front matter too.

## Formal Documents and Specifications

All formal documents and specifications are to be written in LaTeX unless otherwise specified. These documentations are located under *docs* folder.