---
title: "Test paper."
author: Paul Gowder
bibliography: refs.bib
date: November 3, 2018
geometry: margin=1.2in
toc: true
toc_depth: 4
indent: true
fontsize: 12pt
---

I am some text!  Now I will cite a paper: [@gowder2014market] I cited it! 

it seems... and this is very strange... that the following workflow will get a tag going: 

```
git add .
git commit -m "some commit message"
git tag "hereisatag"
git push
git push --tags
```

but only that sequence.  putting the tags or the pushing in any other order won't. 

