Proof of concept for using CI to keep academic documents built from markdown.  just pushes drafts to releases.

next step is to set up tag conditions for deployment so that better bibtex in zotero can be allowed to auto-update and auto-push without triggering new deploys.

tagged builds work 

```
git add .
git commit -m "some commit message"
git tag "hereisatag"
git push
git push --tags
```

or equivalent on ios.  now to figure out how to not build on every trivial commit. 

----

Ok, I've got it under control! The condition `if: tag IS present` only runs CI at all if a tag is present, and then the `on` condition on deploy also pushes a release under those circumstances.
