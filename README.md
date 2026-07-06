# Test Automation Portfolio

A collection of small, focused projects demonstrating test automation
across multiple languages, frameworks, and testing layers — unit, API, UI,
mobile (real devices), load, and visual regression testing.

Each project is intentionally self-contained (its own README, CI pipeline,
and dependencies) rather than one large monorepo, so each can be read,
run, and evaluated independently.

## Projects

| Project | Stack | What it demonstrates |
|---|---|---|
| [PlaywrightTestingShowcase](https://github.com/gillersja1/PlaywrightTestingShowcase) | C#, NUnit, Playwright | Unit, API, and UI tests in one solution; Page Object Model; Allure reporting merged across all three layers; cross-browser CI matrix (Chromium/Firefox/WebKit) |
| [BrowserStackMobileTests](https://github.com/gillersja1/BrowserStackMobileTests) | C#, NUnit, Playwright, BrowserStack | UI tests running on **real mobile devices** (not emulators) via BrowserStack Automate; no BrowserStack-specific test code required |
| [JMeterLoadTestExample](https://github.com/gillersja1/JMeterLoadTestExample) | Apache JMeter | Parameterized load test plan against a REST API; CLI-driven execution with HTML dashboard reporting; on-demand CI workflow with configurable load |
| [PlaywrightTsUiTests](https://github.com/gillersja1/PlaywrightTsUiTests) | TypeScript, Playwright Test | Idiomatic Playwright Test + Page Object Model; cross-browser and mobile-viewport emulation via declarative config; CI with HTML report artifacts |
| [ApplitoolsPlaywrightCSharp](https://github.com/gillersja1/ApplitoolsPlaywrightCSharp) | C#, NUnit, Playwright, Applitools Eyes | AI-powered visual regression testing; Ultrafast Grid rendering across multiple browsers/devices from a single local page load |

## Why these five

Together, these cover the testing layers a QA/SDET role typically touches:

- **Functional correctness** — unit tests (business logic), API tests (contract/behavior), UI tests (end-to-end user flows)
- **Cross-platform coverage** — desktop browsers, real mobile devices, and emulated mobile viewports
- **Non-functional testing** — load/performance testing with JMeter
- **Beyond functional assertions** — visual regression testing catching layout/rendering bugs that behavioral assertions can't

They also intentionally span **two languages** (C# and TypeScript) and
**two visual-testing philosophies** (deterministic pixel/DOM assertions
in the UI suites vs. AI-based visual comparison with Applitools), to show
range rather than depth in only one stack.

## A shared test target

Most of these point at [saucedemo.com](https://www.saucedemo.com/) — a
public demo store built specifically for test automation practice — so
the same application is exercised across nearly every project. That's
deliberate: it makes it easy to compare *how* each tool/framework
approaches the same problem (e.g., compare the Playwright C# UI suite
against the Playwright TypeScript UI suite for the same login flow).

The JMeter project targets [reqres.in](https://reqres.in/), a public test
REST API better suited to load generation than a full web app.

## Where to start

If you're reviewing this portfolio and only have time for one repo,
**PlaywrightTestingShowcase** is the best single entry point — it covers
three testing layers (unit/API/UI) and the most CI/reporting depth in one
place. From there, **ApplitoolsPlaywrightCSharp** and
**BrowserStackMobileTests** each show a different specialized capability
built on the same Playwright/C#/NUnit foundation.

## Running any of these locally

Each project's own README has full setup steps, but at a glance:

- **.NET projects** (`PlaywrightTestingShowcase`, `BrowserStackMobileTests`, `ApplitoolsPlaywrightCSharp`) need the .NET 8 SDK
- **PlaywrightTsUiTests** needs Node.js 18+
- **JMeterLoadTestExample** needs a Java runtime + Apache JMeter on your `PATH`

All five have a GitHub Actions workflow under `.github/workflows/` that
runs on push/PR, so you can also just check each repo's Actions tab
instead of running anything locally.
