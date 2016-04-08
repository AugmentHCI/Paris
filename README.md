## Paris Client Code

This code is based on the Polymer Starter Kit

### Install dependencies

#### Quick-start (for experienced users)

With Node.js installed, run the following one liner from the root of your Polymer Starter Kit download:

```sh
npm install -g gulp bower && npm install && bower install
```

#### Prerequisites (for everyone)

The full starter kit requires the following major dependencies:

- Node.js, used to run JavaScript tools from the command line.
- npm, the node package manager, installed with Node.js and used to install Node.js packages.
- gulp, a Node.js-based build tool.
- bower, a Node.js-based package manager used to install front-end packages (like Polymer).

**To install dependencies:**

1)  Check your Node.js version.

```sh
node --version
```

The version should be at or above 0.12.x.

2)  If you don't have Node.js installed, or you have a lower version, go to [nodejs.org](https://nodejs.org) and click on the big green Install button.

3)  Install `gulp` and `bower` globally.

```sh
npm install -g gulp bower
```

This lets you run `gulp` and `bower` from the command line.

4)  Install the starter kit's local `npm` and `bower` dependencies.

```sh
cd polymer-starter-kit && npm install && bower install
```

This installs the element sets (Paper, Iron, Platinum) and tools the starter kit requires to build and serve apps.

### Development workflow

#### Serve / watch

```sh
gulp serve
```

This outputs an IP address you can use to locally test and another that can be used on devices connected to your network.

#### Run tests

```sh
gulp test:local
```

This runs the unit tests defined in the `app/test` directory through [web-component-tester](https://github.com/Polymer/web-component-tester).

To run tests Java 7 or higher is required. To update Java go to http://www.oracle.com/technetwork/java/javase/downloads/index.html and download ***JDK*** and install it.

#### Build & Vulcanize

```sh
gulp
```

Build and optimize the current project, ready for deployment. This includes vulcanization, image, script, stylesheet and HTML optimization and minification.

## Unit Testing

Web apps built with Polymer Starter Kit come configured with support for [Web Component Tester](https://github.com/Polymer/web-component-tester) - Polymer's preferred tool for authoring and running unit tests. This makes testing your element based applications a pleasant experience.

[Read more](https://github.com/Polymer/web-component-tester#html-suites) about using Web Component tester.

## Dependency Management

Polymer uses [Bower](http://bower.io) for package management. This makes it easy to keep your elements up to date and versioned. For tooling, we use npm to manage Node.js-based dependencies.

Components installed by Bower live in the `app/bower_components` directory. This location is specified by the `.bowerrc` file. Many projects which follow Yeoman conventions place the `bower_components` directory outside of the `app` directory and then mount it using a server. This causes problems for tools like [Vulcanize](https://github.com/polymer/vulcanize) and [web-component-shards](https://github.com/PolymerLabs/web-component-shards) which rely on relative paths. We've chosen to simplify things and have `bower_components` live inside of `app` to resolve these issues.

## Licensing

Like other Google projects, Polymer Starter Kit includes Google license headers at the top of several of our source files. Google's open-source licensing requires that this header be kept in place (sorry!), however we acknowledge that you may need to add your own licensing to files you modify. This can be done by appending your own extensions to these headers.

## Contributing

Polymer Starter Kit is a new project and is an ongoing effort by the Web Component community. We welcome your bug reports, PRs for improvements, docs and anything you think would improve the experience for other Polymer developers.
