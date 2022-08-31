## Run Playwright example tests

**[accessibility](./accessibility/tests/example.spec.ts)** - runs accessibility checks against [https://www.w3.org](https://www.w3.org)

**[android](./android/tests/example.spec.ts)** - runs a basic test using Android's WebView.

**[basic](./basic)** - basic tests to show interactions, element selectors, assertions, upload files, read a response, mock a response, and page object model (POM).

**[chrome-extension](./chrome-extension/tests/example.spec.ts)** - basic test that gets a handle to the background page of Chrome extension.

**[drag-and-drop](./drag-and-drop/tests/example.spec.ts)** - runs example drag-and-drop test utilizing [https://www.w3schools.com/html/html5_draganddrop.asp](https://www.w3schools.com/html/html5_draganddrop.asp).

**[electron](./electron/tests/example.spec.ts)** - runs a basic test for Electron application, controlling main electron process and working with Electron window.

**[fixtures](./fixtures/tests)** - runs example tests utilizing [test and worker fixtures](https://playwright.dev/docs/test-fixtures).

**[github-api](./github-api/tests/example.spec.ts)** - uses GitHub API to test creation of a new repo, bug, and feature, then deletion of repo.

**[oauth](./oauth/tests/example.spec.ts)** - runs oauth tests for LinkedIn, Facebook, and Google, to login to <https://courses.ultimateqa.com/users/sign_in>.

**[performance](./performance/tests/example.spec.ts)** - web performance tests using resource timing API, DevTools, and lighthouse, run against
[https://fastestwebsite.net](https://fastestwebsite.net/)

**[svgomg](./svgomg/tests/example.spec.ts)** - End-to-end tests for SVGOMG! site, hosted at [https://demo.playwright.dev/svgomg](https://demo.playwright.dev/svgomg)

**[todomvc](./todomvc/tests/example.spec.ts)** - End-to-end tests for ToDoMVC site, hosted at [https://demo.playwright.dev/todomvc](https://demo.playwright.dev/todomvc)

**[visual-comparison](./visual-comparison/tests/example.spec.ts)** - visually compares snapshots with golden screenshots and text content for playwright.dev landing page.

## Configuration

The [baseURL](https://playwright.dev/docs/api/class-testoptions#test-options-base-url) value for most tests is set as a [workflow environment variable](https://docs.github.com/en/actions/learn-github-actions/environment-variables). This allows flexibility for the URL of the sites tested. By not hardcoding a URL in `page.goTo('')` we can simply pass baseURL without changing the test script e.g. test.site.com -> stage.site.com -> prod.site.com
