# newer-coder (Apologies to [new-coder](http://newcoder.io)

A New Coder tutorial: 1 Python data visualization tutorial for a new coder with 1-3 semesters of programming experience.

This fork of new-coder will attempt to smooth out many of the common issues my students found last semester with new-coder.io, and will
slow down the pace of the new-coder.io tutorials. The instruction of the tutorials will be less "copy-and-paste", and will involve more 
reflective questions.

It will start with just the data visualization tutorial. 

---- Below is the original README, unchanged ----

General directory layout:

	├── <Project>/
	│   ├── README.md
	│   ├── requirements.txt
	│   ├── lib/
	│   ├── tests/  # only for more advanced tutorials

## CONTRIBUTING


*PLEASE* – When editing tutorial or full source code, please edit the documentation to go along with it within the `website` folder (and vice-versa).

When writing documentation, please use [smart quotes](http://en.wikipedia.org/wiki/Quotation_mark_glyphs). :)


## Documentation Build Instructions

Documentation is essentially the website itself.  Simply install requirements, run the build command within `website` directory:


```bash
$ mkvirtualenv newcoder-website
(newcoder-website) $ cd website
(newcoder-website) $ pip install -r requirements.txt
```

To build the site:

```bash
(newcoder-website) $ mynt gen -f _site
```

To serve the site locally:

```bash
(newcoder-website) $ mynt serve _site
```

And navigate to `localhost:5000`.

I’ve included a simple script that combines the two above commands:

```bash
(newcoder-website) $ ./_local.sh
```

If you get a `permission denied` message, you may need to change the file mode in order to run the `_local.sh` with the `./` preceeding:

```bash
(newcoder-website) $ chmod +x _local.sh
(newcoder-website) $ ./_local.sh
```
