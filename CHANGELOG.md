## HEAD

## 0.3.1 / 2019-10-18

  * documentation: move from zip to tarball archives to allow for installation with `npm install`
  * documentation: add screencast videos
  * refactor: improve the integration of the adblock library provided by the browser [Cliqz](https://cliqz.com/) and better link filtered content to a specific filter in the output
  * documentation: add [FAQ.md](FAQ.md) to answer frequent questions
  * dependency: update version and provider of [puppeteer-har](https://www.npmjs.com/package/puppeteer-har) to [Remove git dependency for end-users](https://github.com/EU-EDPS/website-evidence-collector/issues/9)
  * dependency: downgrade version of tough-cookie to match version employed by chrome-har
  * documentation: add guidance to install unstable versions and to uninstall any version
  * bugfix: make json console output json compliant
  * feature: add secure connection tests

## 0.3.0 / 2019-09-25

  * refactor: rename `collect.js` to `website-evidence-collector.js`
  * feature: make npm setup a symlink to have command `website-evidence-collector` available
  * bugfix: fix bug related to URL
  * documentation: add logo

## 0.2.2 / 2019-07-30

  * bugfix: in some cases, location of JS cookies is not set in its log data
  * documentation: update README.md
  * feature: log commit version if git is installed and repository found

## 0.2.1 / 2019-07-29

  * security: update lodash
  * documentation: update data protection notice in README.md

## 0.2.0 / 2019-07-29

  * license: adopt EUPL license and add headers to relevant files
  * feature: change cookie placement locator mechanism to use injections and stacktrace.js instead of `Debugger.scriptParsed` for improved accuracy
  * feature: also track HTTP cookies
  * feature: record HAR file
  * feature: include all links in output data
  * feature: detect and report use of LocalStorage API
  * feature: employ easyprivacy list to detect potential tracking (beacons, analytics)
  * feature: avoid HeadlessChrome in `UserAgent` when sending requests
  * feature: decode LocalStorage data from JSON if possible
  * feature: record websocket traffic
  * feature: configure output options and introduce silent mode
  * feature: allow browsing of other first-party web pages

## 0.1.0 / 2019-04-17

  * Birthday!
  * move monkey-patched code to a proper repository
  * create README.md and CHANGELOG.md
  * feature: use `Debugger.scriptParsed` and heuristic assumptions to get insights on when cookies are placed
