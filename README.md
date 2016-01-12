# Editing SheffieldUQ pages

These are the webpages for the SheffieldUQ group.

### Getting started

* Tell me your github name so that I can add you to the SheffUQ group.
* Clone the page
```
git clone https://github.com/SheffUQ/SheffUQ.github.io.git
cd SheffUQ.github.io
```
* Checkout the source branch
```
git checkout -b source
```

* Make changes etc.
* Run `jekyll serve` (You must install [jekyll](http://jekyllrb.com/) first).
* Open web browser and enter "http://127.0.0.1:4000/" to see the website.


### Blog entries
* `cd _posts/`
* Create a new file that obeys the naming convention YEAR-MONTH-DATE-NAME.markdown
* You can use [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). I haven't sorted adding latex math equations yet, but I don't think that's hard.



### Updating github

Because we are using [Jekyll-scholar](https://github.com/inukshuk/jekyll-scholar) for the references, updating the pages is slightly convoluted.

There are two branches to the repo - master and source. All the source code lives in the source branch, and the html from the `_site/` directory needs to go into the `master` branch. Once you have built and tested the site locally, 
commit the changes to source branch. Then
[do the following](https://github.com/randymorris/randymorris.github.com/blob/source/README.md) to update the github repo.,

```
git branch -D master
git checkout -b master
git filter-branch --subdirectory-filter _site/ -f
git checkout source
git push --all origin
```

In time I'll see if I can automate this.


### Source
The website uses the [Jekyll-Pithy](https://github.com/smallmuou/Jekyll-Pithy) theme.
