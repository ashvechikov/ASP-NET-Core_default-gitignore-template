ASP NET Core default **.gitignore** file template

To untrack a single file that has already been added to your repo, i.e., stop tracking the file but not delete it from your system use:

```bash
git rm --cached filename
```

To untrack every file that is now in your .gitignore:

First commit any outstanding code changes, and then, run this command:

```bash
git rm -r --cached .
```

This removes any changed files from the index(staging area), then just run:

```bash
git add .
```

Commit it:

```bash
git commit -m "new .gitignore added now"
```

To undo

```bash
git rm --cached filename
```

use

```bash
git add filename.
```
