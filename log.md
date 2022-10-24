# this is log of the site building

## save change in master branch

```shell
git add . && git commit -m 'save change in master branch' && git push
# remove branch
git branch --delete 0v
# create gh-pages branch
git checkout -b gh-pages
git add . && git commit -m 'save change in gh-pages branch' && git push
# this do not work
# use the deploy script that go with this
```
