Test repo
====

### Test: Create a local repo, then link to GitHub.

The following approach worked:

### Create a local repo

Create, add, and commit one or more files to your local repo.

```
mkdir abcd ; cd abcd
git init
touch README.md  (or simply edit)
git add README.md
git commit -m "first commit"
```

### Link the local repo to the remote repo

Link the local repo to the remote repo using `git remote add`.
(More precisely, link the `origin` branch of the local repo.)

```
git remote add origin https://github.com/<yourusername>/abcd.git
```

Push local `master` to the remote `origin`:

```
git push -u origin master
```

Afterward, just `git push` is sufficient.
