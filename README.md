# Editing SheffieldUQ pages

These are the webpages for the SheffieldUQ group.

### Getting started

* Tell me your github name so that I can add you to the SheffUQ group.
* Clone the page
```
git clone https://github.com/rich-d-wilkinson/SheffUQwebpages
cd SheffUQwebpages
```


### Making changes etc.

The structure of the website is defined in /\_includes and /\_layouts.
The site is setup to use markdown. Content lives in .markdown or .md files, such as index.md. These are markdown files, so you don't need to use html tags (see https://daringfireball.net/projects/markdown for example).

Once you've made edits, you'll need to

* Run `jekyll serve --future TRUE` (You must install [jekyll](http://jekyllrb.com/) first).
* Open web browser and enter "http://127.0.0.1:4000/" to see the website.

If that looks okay, commit the code to github,

`git add .
git commit -m 'Description of changes'
git push --set-upstream origin master
`

 and upload it to cpanel.
The html files are those in the  /\_site directory.

`cd _site
ftp username@staff.shef.ac.uk
# enter password
cd public_html
send index.html
send consultancy.html`


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
