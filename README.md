# HTML-TIME

https://setyourwatchby.netlify.com

A ludicrous experiment triggered by a playfull tweet:

> free side project idea: HTML-only static site generated clock that deploys a new version to @netlify every minute
> – [@zachleat](https://twitter.com/zachleat/status/1020034115817680896)


## What does it do?

- It builds a page with the local time for a variety of timezones. (correct at build time.)
- When served on [Netlify](https://www.netlify.com)'s global CDN, visitors are routed to the correct page for them based on the country they access from.

## What on earth for?

Since we can run this build so regularly and with such confidence on Netlify, we rebuild and deploy automatically every minute.

## Are you an idiot?

Possibly. But it turns out that this is a nice example of how the country-specific CDN routing is on Netlify thanks to its concise, yet powerful [`_redirects`](_redirects) API. ([docs](https://www.netlify.com/docs/redirects/))

Have a poke around!


## Developing locally

```
// clone this repository
git clone git@github.com:philhawksworth/html-time.git

// move into the project and install the dependencies
cd html-time
yarn

// run a local development server with auto-rebuild and hot reloading
yarn start
```

## Deployed (really rather often) to Netlify

[![Netlify Status](https://api.netlify.com/api/v1/badges/08fef174-2c11-4911-a610-19a327172024/deploy-status)](https://app.netlify.com/sites/setyourwatchby/deploys)





