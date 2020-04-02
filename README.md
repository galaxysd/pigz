pigz with Blocked GZip Format (BGZF) support

See <https://github.com/madler/pigz/pull/19>.

```
git remote add madler https://github.com/madler/pigz.git
git remote add -t AddBlockCompress-BGZip BGZip https://github.com/JGI-Bioinformatics/pigz.git
git fetch

$ git remote -v
BGZip	https://github.com/JGI-Bioinformatics/pigz.git (fetch)
BGZip	https://github.com/JGI-Bioinformatics/pigz.git (push)
madler	https://github.com/madler/pigz.git (fetch)
madler	https://github.com/madler/pigz.git (push)
origin	git@github.com:galaxysd/pigz.git (fetch)
origin	git@github.com:galaxysd/pigz.git (push)

$ git branch -av
  AddBlockCompress-BGZip                8c92aa3 fixed 0 byte input file and -p 1 compress added more tests for edge cases and gzip compatibility
* madler                                fe822cb pigz version 2.4
  remotes/origin/AddBlockCompress-BGZip 8c92aa3 fixed 0 byte input file and -p 1 compress added more tests for edge cases and gzip compatibility
  remotes/origin/HEAD                   -> origin/AddBlockCompress-BGZip
  remotes/origin/madler                 fe822cb pigz version 2.4

git checkout AddBlockCompress-BGZip
git checkout -b galaxy

# git push --set-upstream origin galaxy
```
