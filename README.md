# Examples for FME Browser SDK and FME JavaScript SDK

[![Documentation](https://img.shields.io/badge/FME_Browser_SDK-documentation-informational)]([https://developer.harness.io/docs/feature-management-experimentation/sdks-and-infrastructure/server-side-sdks/net-sdk/](https://developer.harness.io/docs/feature-management-experimentation/sdks-and-infrastructure/client-side-sdks/browser-sdk)) [![Documentation](https://img.shields.io/badge/FME_JavaScript_SDK-documentation-informational)]([https://developer.harness.io/docs/feature-management-experimentation/sdks-and-infrastructure/server-side-sdks/net-sdk/](https://developer.harness.io/docs/feature-management-experimentation/sdks-and-infrastructure/client-side-sdks/javascript-sdk))

## Table of Contents
**[Intro](#intro)**<br>
**[Requirements](#requirements)**<br>
**[Quickstart](#quickstart)**<br>
**[Further Reading](#further-reading)**<br>

## Intro

These single web page examples show you how to set up the [FME Browser SDK](https://github.com/splitio/javascript-browser-client) and the [FME JavaScript SDK](https://github.com/splitio/javascript-client) to evaluate an FME feature flag and send an event.

![Web page running Browser SDK example](https://github.com/splitio/example-javascript-browser/blob/master/images/example-browser-sdk.png)

The Browser SDK is optimized for web browsers and built on top of the JavaScript SDK core modules. To compare between the SDK versions, see also the [JavaScript to Browser SDK Migration Guide](https://developer.harness.io/docs/feature-management-experimentation/sdks-and-infrastructure/examples/browser-sdk-migration).

## Requirements

To run the example, you need:
* just a web browser
* (optional) [Python](https://www.python.org/downloads/)

## Quickstart

This repo contains three examples:
* `index-js-sdk.html` - shows how to set up the JavaScript SDK
* `index-js-browser-sdk.html` - shows how to set up the Browser SDK (similar to JavaScript SDK, but optimized for web browsers)
* `index-js-browser-sdk-full.html` - shows how to set up the Browser SDK, with logging

To run the SDK on the web page:

1. Log in to [Harness](https://app.harness.io) or create a free account.
1. Navigate to **Feature Management & Experimentation** > **FME Settings** > **Projects** > **View** > **SDK API Keys** and copy a client-side SDK API key for one of your FME environments.
1. Paste your SDK API key as the value of the `sdkKey` variable in the HTML file.
1. Create a feature flag, initiate the FME environment, define the flag's targeting rules, and assign the flag name to the `featureFlagName` variable in the HTML file.
1. Open the HTML file in your browser and see the treatment for the feature flag.
 
 You can also serve the HTML files using Python as a lightweight web server, by running `python3 -m http.server` in a command prompt from your local `example-javascript-browser` folder. Then you can navigate to the pages on `localhost`, for example:
 
 [http://localhost:8000/index-js-browser-sdk.html](http://localhost:8000/index-js-browser-sdk.html)

 ## Further Reading

See the [FME JavaScript SDK](https://developer.harness.io/docs/feature-management-experimentation/sdks-and-infrastructure/client-side-sdks/javascript-sdk) and the [FME Browser SDK](https://developer.harness.io/docs/feature-management-experimentation/sdks-and-infrastructure/client-side-sdks/browser-sdk) docs to learn about configuration options, optimizations, and event tracking.

For more information about feature flags, see our [Feature Management](https://developer.harness.io/docs/feature-management-experimentation/feature-management) documentation.

-------

[Harness](https://harness.io) is an autonomous Software Development Lifecycle Platform that provides software delivery, security testing, runtime protection, and cost management, so your team ships code faster, safer, and smarter.
