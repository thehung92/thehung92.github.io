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
git add . && git commit -m 'save change in news announcement'
bin/deploy -s source -d gh-pages
```

## run the site on local

```shell
git checkout source
bundle exec jekyll serve
# add a favicon.ico # this seem to be the way of webrick
touch favicon.ico
# commit before local test
git add . && git commit -m 'save change in about pages'
bundle exec jekyll serve
# commit before deploy
git add . && git commit -m 'create news announcement'
bin/deploy -s source -d gh-pages
```

