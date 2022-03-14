### Git Commands

```bash
# git log --oneline
97c32d3 (HEAD -> main, origin/main, origin/HEAD) teste
044bd22 new test
afb058c Initial commit
```

```bash
# git log --pretty=short
commit 97c32d37441916d3918c7e579767b32879eaec53 (HEAD -> main, origin/main, origin/HEAD)
Author: Amaury Borges Souza <amaurybsouza@gmail.com>

    teste

commit 044bd22abfe1fa3a468507133e98ee322c746cbc
Author: amaurybsouza <amaurybsouza@gmail.com>

    new test

commit afb058c4b0dacda07266578df6e670a999d86115
Author: Amaury Borges Souza <amaurybsouza@gmail.com>

    Initial commit
```

### How to revert a commit done on the master

- First of all, you need check a `git log` command to check the log of commits

```bash
# git log
```
Now you can proceed:

```bash
# git revert 011b2e306e2edf968820a44b38a5d52d9772c0a
```

OBS: for good practices, NEVER change the history on the master, always use `git revert` command, it's don't change the history.

