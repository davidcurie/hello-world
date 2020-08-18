# About this project
Hello!

I am learning how to use Git. This is a testing directory for learning how to commmit, track changes, and manage push/pull requests.


# Learning Notes

I have copied an index.html file into this repository and created a new branch called `gh-pages`. I have also manually set the default branch in GitHub from `master` to `gh-pages`. This allows me to serve a static landing html page to serve as a mini website by going to `https://username.github.io/repositoryname`. For me this is <https://davidcurie.github.io/hello-world>.

Be sure to also copy in a css file if you want to spice up your plain html.

# Useful resources

- Git-It tutorial: <https://github.com/jlord/git-it-electron>
- GitHub Desktop: <https://desktop.github.com>
- Markdown guide: <https://www.markdownguide.org/basic-syntax/>
- Pandoc: <https://pandoc.org>
- DocOnce: <http://hplgit.github.io/doconce/doc/pub/tutorial/tutorial.html>

## Recommended Reading

### Learning the tools
- GitHub Flow: <https://guides.github.com/introduction/flow/>
- Branching best practices : <https://nvie.com/posts/a-successful-git-branching-model/>
- GitHub Pages: <https://pages.github.com>


### Opinions on editing
- Open-source writing: [Beware the academic hipster](https://labandfield.wordpress.com/2013/08/08/beware-the-academic-hipster-or-use-what-works-for-you/)


### Thesis approaches
- markdown: <https://www.theurbanist.com.au/2018/02/writing-a-thesis-in-markdown/>
    - Text files written in markdown and converted to LaTex pdf with pandoc. Also convertable to .html and .docx
- LaTex + Markdown: <https://tech.lauritz.me/easy-latex-with-markdown-pandoc/>
- Git approach for documents: <https://edit.hypotheses.org/276>


## DocOnce


### Sample output
- Scientific HTML report in markdown: [Github Minimal Theme](http://hplgit.github.io/teamods/writing_reports/_static/report_github_minimal.html)
- Scientific HTML report in bootstrap: [Plain Bootstrap](http://hplgit.github.io/teamods/writing_reports/_static/._report_bootstrap001.html#math:problem)
- Scientific Jupyter Notebook: [iPython](https://nbviewer.jupyter.org/url/hplgit.github.com/teamods/writing_reports/_static/report.ipynb)
- LaTex PDF: [Electronic](http://hplgit.github.io/teamods/writing_reports/_static/report.pdf)
- HTML slides: [deck.js, swiss theme](http://hplgit.github.io/doconce/doc/pub/slides/demo/demo_deck_swiss.html#slide-0)
- LaTex slides: [Beamer](http://hplgit.github.io/doconce/doc/pub/slides/demo/demo_blue_plain.pdf)
- Interactive quiz: [Pure text](http://hplgit.github.io/doconce/doc/pub/quiz/._quiz001.html)
- Complete List: [Scientific Report options](http://hplgit.github.io/teamods/writing_reports/index.html)

## Pandoc

### Useful commands

```
pandoc -t desiredFormat -f oldFormat -o Output Input
```
But pandoc is smart about the -t[o] field and the f[rom] field if you specify extensions in the filenames:

```
pandoc -o Output.pdf Input.md
````
Other options:

- `-s` : standalone file (necessary for html with inserted css)
- `-toc`: table of contents
- `--bibliography=FILE` specify bibliography to include
- `--csl=SOURCE` specifies bibliography style
- `--css=SOURCE` specify stylesheet for html
- `--mathjax` to properly render math equations in html

### More resources

- Citation Style Language Library: <https://github.com/citation-style-language/styles>
- Plain css : [pandoc css](https://gist.github.com/killercup/5917178) 
- Copy and paste the code into a text file with .css extension in the same directory as your instance of pandoc. Then pass the option `--css=yourstylesheet.css -s` at runtime.
- More CSS templates: <https://www.w3schools.com/w3css/w3css_templates.asp>

If you want to modify an existing css file, note that dark-mode overwrites can be addressed in the following way:

```css
@media (prefers-color-scheme: dark){
    body {
        background-color #2f2f2f;
        color: #f0f0f0; }
        
    h1, h2, h3, h4, h5, h6 {
        color: #f0f0f0; }
}
```
