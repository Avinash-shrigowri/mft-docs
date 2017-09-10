# MFT Documentation

The goal of the mft Documentation project is to centralize, automate and modernize the mft documentation authoring, editing and publishing process.

mft-doc is based on [gitbook](https://www.gitbook.com/) and [Markdown](http://daringfireball.net/projects/markdown/syntax).

## Authoring
Due to the popularity of [Markdown](http://daringfireball.net/projects/markdown/syntax), there are many tools to choose from for authoring.
While a simple text editor will work just fine, many prefer tools like [Atom](https://atom.io/), or [StackEdit](https://stackedit.io/).
However, considering that mft-doc is leaning towards the gitbook-way of doing things, authors may wish to consider using the
[gitbook editor](https://www.gitbook.com/editor) for its integration with gitbook conventions and configuration.

## Building

When using tools like the [gitbook editor](https://www.gitbook.com/editor) or [StackEdit](https://stackedit.io/),
you will have the benefit of real-time previews of your work, so building on your local machine will not be necessary. If the need
arises however, you can utilize your local [Development Environment](#development-environment).
If using gitbook editor, be sure to [squash your commits](http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html) before pushing them upstream.

Lastly, mft-doc will be build  continuously `_build` artifacts will be archived once we mature for each build.

## Development Environment
mft-doc is  based on [node](http://nodejs.org/), [npm](https://www.npmjs.com/), [grunt](http://gruntjs.com/),
and [gitbook](https://www.gitbook.com/). Use the following steps to configure your environment for local development.

**NOTE:** These steps are not necessary for simple authoring. See the [Authoring](#authoring) for details.

1. Install node using one of the [provided installers](http://nodejs.org/download/),
[brew](http://thechangelog.com/install-node-js-with-homebrew-on-os-x/), or whatever means you choose.

2. Install the [grunt-cli](http://gruntjs.com/using-the-cli):
```
npm install grunt-cli -g
```

3. Install gitbook-cli:
```
npm install gitbook-cli -g
```

4. Install all project dependencies:
```
npm install
```


5. Serve your gitbook contents locally:
```
cd src
gitbook serve
```
