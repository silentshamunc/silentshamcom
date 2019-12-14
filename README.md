# Silent Sham

****

The Silent Sham website is automatically generated from this repo.

### How to submit a new article about the Silent Sham:

You need to create a free GitHub account (sorry).

1. Go to [this link](https://github.com/silentshamunc/silentshamcom/new/master/site/content).
2. After the `silentshamcom/site/content/`, there's an input box that asks you to "Name your file". Name
   the file something like `2019-12-25-timesgazette.md`. The title isn't actually important, but the `.md`
   at the end is.
3. Underneath "Edit new file", copy and complete the following template.
4. Click the green "Propose new file" button. You can just ignore the text fields under "Propose new file."

Template:

```
---
date: 2019-12-XX
title: 
link: 
source: 
---
```

Your submission needs to be approved before it appears on the site. Thanks for helping keep track of
the endless deluge of bad press around the 2.5 millon dollar Silent Sham.


# Building the website independently

This repo is based on the [victor-hugo](https://github.com/netlify-templates/victor-hugo) template by Netlify.
If, for some reason, you want to build it on your home computer, I guess you can do that.

### :exclamation: Prerequisites

You need to have the latest/LTS [node](https://nodejs.org/en/download/) and [npm](https://www.npmjs.com/get-npm) versions installed in order to use Victor Hugo.

Next step, clone this repository and run:

```bash
npm install
```

This will take some time and will install all packages necessary to run Victor Hugo and its tasks.

### :construction_worker: Development

While developing your website, use:

```bash
npm start
```

or for developing your website with `hugo server --buildDrafts --buildFuture`, use:

```bash
npm run preview
```

Then visit http://localhost:3000/ _- or a new browser windows popped-up already -_ to preview your new website. Webpack Dev Server will automatically reload the CSS or refresh the whole page, when stylesheets or content changes.

### :package: Static build

To build a static version of the website inside the `/dist` folder, run:

```bash
npm run build
```

To get a preview of posts or articles not yet published, run:

```bash
npm run build:preview
```

See [package.json](package.json#L8) for all tasks.

