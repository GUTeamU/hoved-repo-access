hoved-repo-access
=================

Add this to your `~/.ssh/config` for convenience:

```
Host sibu
  Hostname sibu.dcs.gla.ac.uk
  User YOUR_MATRIC_NUMBER
Host hovedgit
  Hostname localhost
  Port 9999
  User YOUR_MATRIC_NUMBER
```

Set up a tunnel:
```bash
ssh -L9999:hoved:22 sibu
```

Clone the repository:
```bash
git clone hovedgit:/extra/2013/u/git/REPO_NAME
```
