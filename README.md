# Track-Spense

<p align="center">
  <strong>Track Smart. Spend Better.</strong><br />
  A thoughtful, privacy-first way to understand your money.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?logo=android&logoColor=white" alt="Android" />
  <img src="https://img.shields.io/badge/Language-Kotlin-7F52FF?logo=kotlin&logoColor=white" alt="Kotlin" />
  <img src="https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4?logo=jetpackcompose&logoColor=white" alt="Jetpack Compose" />
  <img src="https://img.shields.io/badge/Storage-Room-6D4C41" alt="Room" />
  <img src="https://img.shields.io/badge/Privacy-Local%20first-590907" alt="Local first" />
</p>

---

## Overview

Track-Spense is an Android personal-finance tracker designed to help people record, organize, and review everyday money activity. It brings accounts, transactions, category spending, and financial summaries into one focused experience.

The app is built around a local-first approach: financial records are stored on the device rather than sent to a company-operated financial database.

## Product principles

- **Clarity first** — make income, expenses, balances, and spending patterns easy to understand.
- **Local-first privacy** — keep personal financial records on the device.
- **Real data only** — do not populate production accounts with invented balances, sample transactions, or demo analytics.
- **Reliable calculations** — derive summaries from persisted transactions and account records.
- **Simple by design** — keep everyday tracking approachable and uncluttered.

## Features

The application is being developed around the following capabilities. Availability may vary by build.

- Record and manage income and expense transactions.
- Organize spending by category and review category totals.
- Manage multiple bank or cash accounts.
- Review transaction history and search recorded activity.
- View account balances and financial summaries calculated from actual records.
- Browse transactions by date and use calendar-based filtering.
- Support light and dark appearance modes.
- Export financial records for personal backup and review.

## Privacy and data handling

Track-Spense follows a local-first storage model.

- Financial records are stored locally on the device using the app's local database.
- The app does not require a company-hosted financial database for ordinary transaction tracking.
- No bank connection should be inferred from entering a bank name or account label.
- Import, export, SMS, notification, or other optional capabilities must operate only with the permissions and user actions required by Android and applicable distribution policies.
- Never add real account numbers, card numbers, PINs, CVVs, passwords, or OTPs to issues, screenshots, logs, or source control.

Review the in-app privacy disclosures and the published privacy policy for the exact data practices of the version you install.

## Technology

| Area | Technology |
| --- | --- |
| Platform | Android |
| Language | Kotlin |
| UI | Jetpack Compose |
| Local persistence | Room |
| Reactive UI state | Kotlin Flow and Compose state |
| Background scheduling | WorkManager, where applicable |
| Build system | Gradle |

## Project structure

This repository contains the Android application source. The exact module and package structure may evolve as development continues.

Typical Android project areas include:

- `app/` — application module, source code, resources, and build configuration.
- `gradle/` — Gradle wrapper and dependency configuration.
- `build.gradle.kts` and settings files — project build configuration.

## Getting started

### Requirements

- Android Studio with a compatible Android Gradle Plugin and Kotlin toolchain.
- A compatible JDK configured for the project.
- Android SDK versions required by the app module.

### Open the project

1. Clone this repository.
   ```bash
   git clone https://github.com/vtcxxager/spendwith.git
   ```
2. Open the cloned folder in Android Studio.
3. Allow Gradle sync to complete.
4. Select the `app` run configuration.
5. Run the application on an emulator or Android device.

Use the Gradle wrapper included in the repository for command-line builds:

```bash
# Windows
.\\gradlew.bat assembleDebug

# macOS / Linux
./gradlew assembleDebug
```

## Screenshots

Screenshots and product walkthroughs will be added here as the public release assets are prepared.

## Release builds

Release bundles are generated from Android Studio using **Build → Generate Signed App Bundle or APK → Android App Bundle** and the `release` variant.

Signing credentials are private. Never commit upload keystores, signing passwords, API secrets, local properties containing secrets, or private certificates to this repository. Keep secure backups of signing material outside source control.

## Contributing

This repository is maintained for the Track-Spense project. Before proposing changes:

1. Keep financial calculations based on persisted, genuine records.
2. Avoid adding mock financial data to production code paths.
3. Preserve local-first data handling unless the product's privacy model is explicitly revised.
4. Test database migrations and date/time behavior when changing persistence or transaction logic.
5. Do not include personal financial information in commits, issues, or test fixtures.

## License

No open-source license has been specified yet. Unless a license is added to this repository, the source remains under the copyright owner's all-rights-reserved terms. Do not assume it is available for reuse, redistribution, or commercial use.

---

<p align="center">
  <strong>Track-Spense</strong><br />
  Track Smart. Spend Better.
</p>
