Useful-GitHub-Commands
======================

A set of useful github commands I use on a regular basis

* Make a new repo:

```sh
curl -u 'USER' https://api.github.com/user/repos -d '{"name":"REPO"}'
```

Remember replace USER with your username and REPO with your repository/application name!

```sh 
Example: curl -u 'ayp1359' https://api.github.com/user/repos -d '{"name":"CodePath-Twitter","description":"CodePath training at FB"}'
```

* Remove the git in current directory:
```sh
rm -rf .git
```

* To add files:
```sh
git init
git add .
git commit -m "Initial commit"
git remote add origin <project url>
git push -f origin master
```

* To remove files:
```sh
git rm $(git ls-files --deleted)  
```
* Create a .tar.gz file of git:
```sh
git archive HEAD | gzip > archive.tar.gz
git archive master --format=zip --output=./archive.zip
```

* Garbage collection (run occasionally to optimize performance)
```sh
git gc
```
