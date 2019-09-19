# get-time-between

> Measure the amount of time during work hours between two dates

[![NPM version](http://img.shields.io/npm/v/get-time-between.svg?style=flat-square)](https://www.npmjs.com/package/get-time-between) [![NPM downloads](http://img.shields.io/npm/dm/get-time-between.svg?style=flat-square)](https://www.npmjs.com/package/get-time-between) [![Build Status](http://img.shields.io/travis/JamieMason/get-time-between/master.svg?style=flat-square)](https://travis-ci.org/JamieMason/get-time-between) [![Maintainability](https://api.codeclimate.com/v1/badges/80461b911c6c624194a2/maintainability)](https://codeclimate.com/github/JamieMason/get-time-between/maintainability)

## Table of Contents

-   [🌩 Installation](#-installation)
-   [📝 API](#-api)
-   [👏🏻 Credits](#-credits)
-   [🙋🏾‍♂️ Getting Help](#♂️-getting-help)
-   [👀 Other Projects](#-other-projects)
-   [🤓 Author](#-author)

## 🌩 Installation

    npm install --save get-time-between

## 📝 API

Calculate the number of millseconds during working hours between two dates. The result of this can be formatted as you wish, with libraries such as [`pretty-ms`](https://github.com/sindresorhus/pretty-ms) for example.

All methods take an optional 3rd argument containing the following options, shown here with their default values:

```js
import { getTimeBetween } from "get-time-between";

const fridayFivePm = new Date("May 17 2019 17:00:00");
const mondayElevenAm = new Date("May 20 2017 11:00:00");

const timeBetween = getTimeBetween(fridayFivePm, mondayElevenAm, {
  dailyEnd: [18, 0, 0], // [hour, minute, second] of the end of included days
  dailyStart: [10, 0, 0], // [hour, minute, second] of the start of included days
  excludedDays: [6, 0] // excluded days of the week (0-6 starting Sunday)
});

console.log(timeBetween);
// => 7200000
```

## 👏🏻 Credits

This project is a fork of <https://github.com/tal/time-between> by [Tal Atlas](https://github.com/tal).

## 🙋🏾‍♂️ Getting Help

Get help with issues by creating a [Bug Report] or discuss ideas by opening a [Feature Request].

[bug report]: https://github.com/JamieMason/get-time-between/issues/new?template=bug_report.md

[feature request]: https://github.com/JamieMason/get-time-between/issues/new?template=feature_request.md

## 👀 Other Projects

If you find my Open Source projects useful, please share them ❤️

-   [**add-matchers**](https://github.com/JamieMason/add-matchers)<br>Write useful test matchers compatible with Jest and Jasmine.
-   [**eslint-formatter-git-log**](https://github.com/JamieMason/eslint-formatter-git-log)<br>ESLint Formatter featuring Git Author, Date, and Hash
-   [**eslint-plugin-move-files**](https://github.com/JamieMason/eslint-plugin-move-files)<br>Move and rename files while keeping imports up to date
-   [**eslint-plugin-prefer-arrow-functions**](https://github.com/JamieMason/eslint-plugin-prefer-arrow-functions)<br>Convert functions to arrow functions
-   [**image-optimisation-tools-comparison**](https://github.com/JamieMason/image-optimisation-tools-comparison)<br>A benchmarking suite for popular image optimisation tools.
-   [**ImageOptim-CLI**](https://github.com/JamieMason/ImageOptim-CLI)<br>Automates ImageOptim, ImageAlpha, and JPEGmini for Mac to make batch optimisation of images part of your automated build process.
-   [**is-office-hours**](https://github.com/JamieMason/is-office-hours#readme)<br>Determine whether a given date is within office hours
-   [**Jasmine-Matchers**](https://github.com/JamieMason/Jasmine-Matchers)<br>Write Beautiful Specs with Custom Matchers
-   [**jest-fail-on-console-reporter**](https://github.com/JamieMason/jest-fail-on-console-reporter#readme)<br>Disallow untested console output produced during tests
-   [**karma-benchmark**](https://github.com/JamieMason/karma-benchmark)<br>Run Benchmark.js over multiple Browsers, with CI compatible output
-   [**karma-jasmine-matchers**](https://github.com/JamieMason/karma-jasmine-matchers)<br>A Karma plugin - Additional matchers for the Jasmine BDD JavaScript testing library.
-   [**logservable**](https://github.com/JamieMason/logservable)<br>git log as an observable stream of JSON objects
-   [**self-help**](https://github.com/JamieMason/self-help#readme)<br>Interactive Q&A Guides for Web and the Command Line
-   [**syncpack**](https://github.com/JamieMason/syncpack#readme)<br>Manage multiple package.json files, such as in Lerna Monorepos and Yarn Workspaces

## 🤓 Author

<img src="https://www.gravatar.com/avatar/acdf106ce071806278438d8c354adec8?s=100" align="left">

I'm [Jamie Mason] from [Leeds] in England, I began Web Design and Development in 1999 and have been Contracting and offering Consultancy as Fold Left Ltd since 2012. Who I've worked with includes [Sky Sports], [Sky Bet], [Sky Poker], The [Premier League], [William Hill], [Shell], [Betfair], and Football Clubs including [Leeds United], [Spurs], [West Ham], [Arsenal], and more.

<div align="center">

[![Follow JamieMason on GitHub][github badge]][github]      [![Follow fold_left on Twitter][twitter badge]][twitter]

</div>

<!-- images -->

[github badge]: https://img.shields.io/github/followers/JamieMason.svg?style=social&label=Follow

[twitter badge]: https://img.shields.io/twitter/follow/fold_left.svg?style=social&label=Follow

<!-- links -->

[arsenal]: https://www.arsenal.com

[betfair]: https://www.betfair.com

[github]: https://github.com/JamieMason

[jamie mason]: https://www.linkedin.com/in/jamiemasonleeds

[leeds united]: https://www.leedsunited.com/

[leeds]: https://www.instagram.com/visitleeds

[premier league]: https://www.premierleague.com

[shell]: https://www.shell.com

[sky bet]: https://www.skybet.com

[sky poker]: https://www.skypoker.com

[sky sports]: https://www.skysports.com

[spurs]: https://www.tottenhamhotspur.com

[twitter]: https://twitter.com/fold_left

[west ham]: https://www.whufc.com

[william hill]: https://www.williamhill.com
