# Josh Giller | Quality Analyst & Test Automation Engineer

I help teams build confidence in software by testing behavior across unit, API, UI, real mobile devices, performance, and visual quality. This portfolio demonstrates hands-on quality analysis and automation engineering across C#, TypeScript, and Kotlin, with CI pipelines and reporting that make results actionable.

📄 [LinkedIn](https://www.linkedin.com/in/josh-giller/)

📊 [Live test dashboard](https://azureteal56.grafana.net/public-dashboards/75e468f01dbe46d39825dd87a9c6d1a6): pass rates, failures, flaky tests and load-test results from every repo below, updated on each CI run

## Skills at a glance

| Skill | Where to see it |
|---|---|
| UI automation (Playwright, Selenium) | [PlaywrightTestingShowcase](https://github.com/gillersja1/PlaywrightTestingShowcase), [PlaywrightTsUiTests](https://github.com/gillersja1/PlaywrightTsUiTests), [SeleniumCSharpUiTests](https://github.com/gillersja1/SeleniumCSharpUiTests) |
| API testing | [PlaywrightTestingShowcase](https://github.com/gillersja1/PlaywrightTestingShowcase) (Playwright API), [PostmanReports](https://github.com/gillersja1/PostmanReports) (Postman/Newman) |
| Contract testing | [PactContractTestingExample](https://github.com/gillersja1/PactContractTestingExample) (Pact, consumer-driven) |
| Real-device mobile testing | [BrowserStackMobileTests](https://github.com/gillersja1/BrowserStackMobileTests) |
| Native Android app & tests | [CollectorsTrackingApp](https://github.com/gillersja1/CollectorsTrackingApp) |
| Visual regression | [ApplitoolsPlaywrightCSharp](https://github.com/gillersja1/ApplitoolsPlaywrightCSharp) |
| Accessibility | [PlaywrightTestingShowcase](https://github.com/gillersja1/PlaywrightTestingShowcase) |
| Test strategy | [PlaywrightTestingShowcase/docs/TEST_STRATEGY.md](https://github.com/gillersja1/PlaywrightTestingShowcase/blob/main/docs/TEST_STRATEGY.md): risk-based coverage, flaky-test policy, defect triage |
| Performance / load | [JMeterLoadTestExample](https://github.com/gillersja1/JMeterLoadTestExample), [K6LoadTestExample](https://github.com/gillersja1/K6LoadTestExample) |
| CI/CD & reporting | GitHub Actions in every repo; Allure, Playwright HTML, JMeter dashboards |
| Observability | Every repo's CI test results sent to one Grafana Cloud dashboard over OpenTelemetry ([test-results-otel](https://github.com/gillersja1/test-results-otel), [live dashboard](https://azureteal56.grafana.net/public-dashboards/75e468f01dbe46d39825dd87a9c6d1a6)) |
| Secret hygiene | gitleaks secret scanning in CI ([BrowserStackMobileTests](https://github.com/gillersja1/BrowserStackMobileTests)) |

## Projects

| Project | Stack | What it demonstrates | CI |
|---|---|---|---|
| [PlaywrightTestingShowcase](https://github.com/gillersja1/PlaywrightTestingShowcase) | C#, NUnit, Playwright | Unit, API, and UI tests in one solution; Page Object Model; Allure reporting merged across all three layers; cross-browser CI matrix (Chromium/Firefox/WebKit) | [![CI](https://github.com/gillersja1/PlaywrightTestingShowcase/actions/workflows/ci.yml/badge.svg)](https://github.com/gillersja1/PlaywrightTestingShowcase/actions/workflows/ci.yml) |
| [PlaywrightTsUiTests](https://github.com/gillersja1/PlaywrightTsUiTests) | TypeScript, Playwright Test | Idiomatic Playwright Test + Page Object Model; cross-browser and mobile-viewport emulation via declarative config; CI with HTML report artifacts | [![CI](https://github.com/gillersja1/PlaywrightTsUiTests/actions/workflows/playwright.yml/badge.svg)](https://github.com/gillersja1/PlaywrightTsUiTests/actions/workflows/playwright.yml) |
| [BrowserStackMobileTests](https://github.com/gillersja1/BrowserStackMobileTests) | C#, NUnit, Playwright, BrowserStack | UI tests running on **real mobile devices** (not emulators) via BrowserStack Automate; credentials kept in CI secrets with a gitleaks scan on every push | [![CI](https://github.com/gillersja1/BrowserStackMobileTests/actions/workflows/browserstack-mobile.yml/badge.svg)](https://github.com/gillersja1/BrowserStackMobileTests/actions/workflows/browserstack-mobile.yml) |
| [ApplitoolsPlaywrightCSharp](https://github.com/gillersja1/ApplitoolsPlaywrightCSharp) | C#, NUnit, Playwright, Applitools Eyes | AI-powered visual regression testing; Ultrafast Grid rendering across multiple browsers/devices from a single local page load | [![CI](https://github.com/gillersja1/ApplitoolsPlaywrightCSharp/actions/workflows/applitools-visual-tests.yml/badge.svg)](https://github.com/gillersja1/ApplitoolsPlaywrightCSharp/actions/workflows/applitools-visual-tests.yml) |
| [SeleniumCSharpUiTests](https://github.com/gillersja1/SeleniumCSharpUiTests) | C#, NUnit, Selenium WebDriver | The same kind of UI suite built with Selenium, for direct comparison against the Playwright C# suite; Selenium Manager handles driver binaries automatically | [![CI](https://github.com/gillersja1/SeleniumCSharpUiTests/actions/workflows/selenium-tests.yml/badge.svg)](https://github.com/gillersja1/SeleniumCSharpUiTests/actions/workflows/selenium-tests.yml) |
| [JMeterLoadTestExample](https://github.com/gillersja1/JMeterLoadTestExample) | Apache JMeter, Node.js | Parameterized load test plan against a local reqres-compatible mock API; CI fails the build on latency or error-rate thresholds; HTML dashboard reporting | [![CI](https://github.com/gillersja1/JMeterLoadTestExample/actions/workflows/load-test.yml/badge.svg)](https://github.com/gillersja1/JMeterLoadTestExample/actions/workflows/load-test.yml) |
| [K6LoadTestExample](https://github.com/gillersja1/K6LoadTestExample) | Grafana k6, JavaScript | The same load test written as code: ramping scenario, per-endpoint checks, and thresholds (with early abort) defined in the script; HTML dashboard and job-summary report in CI | [![CI](https://github.com/gillersja1/K6LoadTestExample/actions/workflows/k6-load-test.yml/badge.svg)](https://github.com/gillersja1/K6LoadTestExample/actions/workflows/k6-load-test.yml) |
| [PostmanReports](https://github.com/gillersja1/PostmanReports) | Postman, Newman, GitHub Actions | API test collection (37 requests, 53 assertions) run with Newman in CI; real API defects tracked in a non-blocking Known Defects folder; HTML and JUnit reports | [![CI](https://github.com/gillersja1/PostmanReports/actions/workflows/github-actions-demo.yml/badge.svg)](https://github.com/gillersja1/PostmanReports/actions/workflows/github-actions-demo.yml) |
| [PactContractTestingExample](https://github.com/gillersja1/PactContractTestingExample) | C#, NUnit, PactNet, ASP.NET Core | Consumer-driven contract tests: the consumer generates a pact against a mock server, the provider verifies the real API against it in CI; includes tests proving a renamed field breaks the contract and an added field does not | [![CI](https://github.com/gillersja1/PactContractTestingExample/actions/workflows/contract-tests.yml/badge.svg)](https://github.com/gillersja1/PactContractTestingExample/actions/workflows/contract-tests.yml) |
| [NeverDeliverShopTests](https://github.com/gillersja1/NeverDeliverShopTests) | TypeScript, Playwright Test | Purchase-flow tests against a satirical "never deliver" e-commerce demo site, using role- and text-based locators | [![CI](https://github.com/gillersja1/NeverDeliverShopTests/actions/workflows/playwright.yml/badge.svg)](https://github.com/gillersja1/NeverDeliverShopTests/actions/workflows/playwright.yml) |
| [test-results-otel](https://github.com/gillersja1/test-results-otel) | Python, GitHub Actions, OpenTelemetry, Grafana | A reusable GitHub Action that turns TRX, JUnit, k6 and JMeter results into OpenTelemetry logs and metrics; every repo here sends its CI results to one Grafana dashboard (pass rate, failures with run links, flaky and slowest tests, known defects, load-test checks) | [![CI](https://github.com/gillersja1/test-results-otel/actions/workflows/ci.yml/badge.svg)](https://github.com/gillersja1/test-results-otel/actions/workflows/ci.yml) |
| [CollectorsTrackingApp](https://github.com/gillersja1/CollectorsTrackingApp) | Kotlin, Android, Room, Firebase | An Android app I built and test myself — unit and instrumented tests, with CI building the APK on every push | [![CI](https://github.com/gillersja1/CollectorsTrackingApp/actions/workflows/android.yml/badge.svg)](https://github.com/gillersja1/CollectorsTrackingApp/actions/workflows/android.yml) |

## Quality engineering focus

These projects show how I approach quality from multiple angles:

- **Analyze behavior at multiple layers** — unit, API, contract, and end-to-end checks help pinpoint where a defect occurs
- **Assess platform and device coverage** — desktop browsers, real mobile devices, and mobile viewport emulation
- **Evaluate non-functional quality** — load testing with pass/fail thresholds in two tools (JMeter and k6), plus accessibility checks
- **Catch visual regressions** — AI-based visual comparison complements functional assertions
- **Make feedback useful** — CI workflows and test reports help teams review outcomes and investigate failures, and one dashboard tracks pass rates, flaky tests and known defects across every repo

They also intentionally span **three languages** (C#, TypeScript, and
Kotlin) and **two browser automation tools** (Playwright and Selenium
WebDriver), to show range rather than depth in only one stack.

## A shared test target

Most of the web UI suites point at [saucedemo.com](https://www.saucedemo.com/) —
a public demo store built specifically for test automation practice — so
the same application is exercised across several projects. That makes it
easy to compare *how* each tool/framework approaches the same problem
(e.g., the Playwright C# UI suite vs. the Playwright TypeScript UI suite vs.
the Selenium suite, testing the same login flow).

## Where to start

If you only have time for one repo, **PlaywrightTestingShowcase** is the
best entry point — it covers three testing layers (unit/API/UI) and the
most CI/reporting depth in one place. From there,
**ApplitoolsPlaywrightCSharp** and **BrowserStackMobileTests** each show a
different specialized capability built on the same Playwright/C#/NUnit
foundation, and **JMeterLoadTestExample**/**K6LoadTestExample** show
the same load test built in a GUI tool vs. written as code.
