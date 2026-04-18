# Maestro Android UI Automation (ApiDemos)

This project demonstrates mobile UI automation using **Maestro** on an Android emulator with the **ApiDemos** sample application.

---

## Overview

The test automates the following flow:

- Launches the ApiDemos app
- Navigates to: Views → Controls → 1. Light Theme

- Enters text into the input field
- Validates that the entered text is visible

The project uses **modular flows (`runFlow`)** for better structure and reusability.

---

## Tech Stack

- Maestro CLI (v2.4.0)
- Android Emulator (Pixel 2 API 33)
- Android Studio (for emulator)
- GitHub Actions (CI/CD)

---

## Project Structure

```text
maestro-project/
apk/
  ApiDemos-debug.apk
tests/
  first-test.yaml
  go-to-light-theme.yaml
  input-text-flow.yaml
.maestro/
  screenshots/
```
## Install Maestro
curl -Ls https://get.maestro.mobile.dev | bash -s -- --version 2.4.0

- Verify installation:

    maestro --version
    
- Run Tests Locally from project root: 
    
    maestro test tests/first-test.yaml
