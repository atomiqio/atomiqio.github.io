---
layout: page
title: Installing Atomiq
menu: starter
lang: en
redirect_from: "/starter/installing.html"
---

# Installing

Atomiq works with [Node.js](https://nodejs.org/) v4.x and v5.x. You can confirm the version you have installed by entering the following command in your terminal.

```
$ node -v
```

The current version uses a generator tool called [yeoman](http://yeoman.io/) to scaffold an Atomiq project. You need to install yeoman and then the atomiq generator.

```
$ npm install -g yo
$ npm install -g generator-atomiq
```

Once you have done this, you can generate new Atomiq projects from your terminal.

```
$ yo atomiq
```

You will be prompted to enter a name for your project. Enter a name and press RETURN.

After Atomiq creates the project, you can `cd` to the directory.
