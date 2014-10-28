Useful-GitHub-Commands
======================

A set of useful github commands I use on a regular basis

GITHUB STUFF
Make a new repo:
curl -u 'USER' https://api.github.com/user/repos -d '{"name":"REPO"}'
# Remember replace USER with your username and REPO with your repository/application name!
Example: curl -u 'ayp1359' https://api.github.com/user/repos -d '{"name":"CodePath-Twitter","description":"CodePath training at FB"}'

git remote add origin git@github.com:USER/REPO.git
git push origin master

to add files:
git init
git add .
git commit -m "Initial commit"
git remote add origin <project url>
git push -f origin master

to remove files:
git rm $(git ls-files --deleted)  
