# Silent Sham

The Silent Sham website is automatically generated from this repo.

### How to submit a new article about the Silent Sham:

You need to create a free GitHub account (sorry).

1. Go to [this link](https://github.com/silentshamunc/silentshamcom/new/master/site/content/links).
2. After the `silentshamcom/site/content/`, there's an input box that asks you to "Name your file". If
   the article was published on Christmas in the Charlotte Weekly, name
   the file something like `2019-12-25-charlotteweekly.md`. The `.md`
   at the end is important.
3. Underneath "Edit new file", copy and complete the following template.
4. Click the green "Propose new file" button. You can just ignore the text fields under "Propose new file."

Template:

```
---
date: 2019-12-XX
title: 
link: 
source: 
cases:
tags:
---
```

Here's an example:

```
---
date: 2019-12-13
title: "'Silent Sam' deal cost UNC-CH a $1.5M grant from major foundation donor"
source: WRAL
link: https://www.wral.com/silent-sam-deal-cost-unc-ch-a-1-5m-grant-from-major-foundation-donor/18830069/
tags:
 - donors
cases:
 - shamsettlement
---
```

Current tags:

 * `75kgiveaway` - what on earth was going on with that $74,999 payment?
 * `allison` - articles mentioning Darrell Allison
 * `baddour` - articles mentioning Judge R. Allen Baddour
 * `cooper` - articles mentioning Roy Cooper
 * `donors` - stories about lost donations to UNC or UNC-CH due to the sham settlement (especially the Mellon Foundation $1.5 grant)
 * `fetzer` - articles mentioning Tom Fetzer
 * `goolsby` - articles mentioning Thom Goolsby
 * `guskiewicz` - articles mentioning Kevin Guskiewicz
 * `holmes` - articles mentioning Jim Holmes
 * `lawcom` - stories mentioning the Lawyer's Committee
 * `loloped` - the December 16 op-ed by BOG members
 * `murphy` - articles mentioning Wendy Murphy
 * `ncscv` - stories mentioning North Carolina Sons of Confederate Veterens (most of them, but it would be a good place to put stuff like https://projects.propublica.org/nonprofits/organizations/581329948)
 * `nelson` - articles mentioning Anna Nelson
 * `powers` - articles mentioning David Powers
 * `ramsey` - articles mentioning Randy Ramsey
 * `randazza` - stories mentioning Marc Randazza
 * `roper` - articles mentioning William Roper
 * `rucho` - articles mentioning Bob Rucho
 * `shanahan` - stories mentioning Tom Shanahan
 * `stein` - articles mentioning NC Attorney General Josh Stein
 * `sturges` - stories mentioning SCV maybe-maybe-not lawyer Boyd Sturges
 * `stone` - stories mentioning NCSCV "commander" Kevin Stone
 * `tgd` - stories mentioning TGD
 * `trust` - stories that mention the Monument Trust
 * `udc` - articles mentioning the United Daughters of the Confederacy
 * `victoryletter` - stories mentioning Kevin Stone's "victory letter"
 * `vroom` - stories mentioning Stone's motorcycle fun times
 * `wolman` - stories mentioning Jay Wolman
 * `womble` - stories mentioning Womble Bond Dickinson

Current cases:

 * `shamsettlement` - the start that started it all
 * `dmca` - the DMCA countersuit

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

