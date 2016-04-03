## League Fun Tournament

### Included out of the box:

A polymer based webapp to help organize the BBK Esports League Fun Tournament Spring 2016.

### Install dependencies

With Node.js installed, run the following one liner from the root of your Polymer Starter Kit download:

```sh
npm install -g gulp bower && npm install && bower install
```

### Development workflow

#### Serve / watch

```sh
gulp serve
```

This outputs an IP address you can use to locally test and another that can be used on devices connected to your network.

#### Build & Vulcanize

```sh
gulp
```

Build and optimize the current project, ready for deployment. This includes vulcanization, image, script, stylesheet and HTML optimization and minification.

## Deploy

### Github Pages

1. Uncomment this line  `// app.baseUrl = '/polymer-starter-kit/';` in app.js near the top
2. Change `app.baseUrl = '/polymer-starter-kit/';`  to `app.baseUrl = '/your-pathname/';` (ex: if you repo is `github.com/username/bobs-awesome-site` you would change this to `bobs-awesome-site`)
3. Run `gulp build-deploy-gh-pages` from command line
4. To see changes wait 1-2 minutes then load Github pages for your app (ex: https://polymerelements.github.io/polymer-starter-kit/)

[See more details](/docs/deploy-to-github-pages.md/)

### I'm having trouble getting Vulcanize to fully build my project on Windows. Help?

Some Windows users have run into trouble with the `elements.html` file in their `dist` folder
not being correctly vulcanized. This can happen if your project is in a folder with a name containing a
space. You can work around this issue by ensuring your path doesn't contain one.

There is also an [in-flight](https://github.com/PolymerElements/polymer-starter-kit/issues/62#issuecomment-108974016) issue
where some are finding they need to disable the `inlineCss` option in our configuration for Vulcanize
to correctly build. We are still investigating this, however for the time-being use the workaround if
you find your builds getting stuck here.

## Licensing

Like other Google projects, Polymer Starter Kit includes Google license headers at the top of several of our source files. Google's open-source licensing requires that this header be kept in place (sorry!), however we acknowledge that you may need to add your own licensing to files you modify. This can be done by appending your own extensions to these headers.
