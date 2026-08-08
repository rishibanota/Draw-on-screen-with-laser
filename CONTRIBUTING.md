# Contributing to Draw On Screen With Laser 🎯

Thank you for your interest in contributing to **Draw On Screen With Laser**! We welcome contributions from developers, designers, testers, and documentation writers of all experience levels.

By participating in this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md).

---

## 📋 Table of Contents

- [How Can I Contribute?](#-how-can-i-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Submitting Pull Requests](#submitting-pull-requests)
- [Development Setup](#-development-setup)
- [Git Commit Guidelines](#-git-commit-guidelines)
- [Pull Request Process](#-pull-request-process)
- [Code Style & Best Practices](#-code-style--best-practices)
- [License](#-license)

---

## 🤝 How Can I Contribute?

### Reporting Bugs

Before creating a bug report, please check the [existing issues](https://github.com/rishibanota/draw-on-screen-with-laser/issues) to avoid duplicate submissions. 

When creating a bug report, please use our **Bug Report Template** and include:
- A clear and descriptive title.
- Steps to reproduce the problem.
- Expected behavior vs. actual behavior.
- Android device model, Android OS version, and screen resolution.
- Screenshots, recordings, or logcat output if applicable.

### Suggesting Enhancements

We are always eager to make **Draw On Screen With Laser** better! If you have ideas for new tools, UI improvements, or performance enhancements:
- Check existing feature requests to make sure it hasn't been proposed yet.
- Open a feature request using our **Feature Request Template**.
- Provide a clear rationale for why this feature would be beneficial to users.

### Submitting Pull Requests

1. **Fork** the repository and clone your fork locally.
2. Create a new topic branch (e.g., `feature/custom-brush-size` or `fix/laser-fade-timer`).
3. Make your changes and commit with meaningful commit messages.
4. Test your changes on an emulator or physical Android device.
5. Push your branch to GitHub and open a **Pull Request** against the `main` branch.

---

## 🛠️ Development Setup

To build and run **Draw On Screen With Laser** locally:

### Prerequisites
- **Android Studio** (Hedgehog / Iguana or newer recommended)
- **Android SDK** (API Level 24+ / Android 7.0 minimum support, targeting API 34+)
- **JDK 17** or compatible Java Development Kit
- Physical Android device or Android Emulator with **Display over other apps** (System Alert Window) permission enabled.

### Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/rishibanota/draw-on-screen-with-laser.git
   cd draw-on-screen-with-laser
   ```
2. Open the project folder in **Android Studio** / VS Code.
3. Sync Gradle project files and ensure all dependencies resolve cleanly.
4. Connect your Android device via USB (with USB Debugging enabled) or start an emulator.
5. Run the application from Android Studio (`Shift + F10` or click **Run**).

---

## 🌿 Branch Naming Conventions

Use clear branch names formatted as:
- `feature/short-description` for new features (e.g., `feature/spotlight-mode`)
- `fix/short-description` for bug fixes (e.g., `fix/overlay-dock-snap`)
- `docs/short-description` for documentation improvements (e.g., `docs/update-readme`)
- `refactor/short-description` for code cleanup or refactoring

---

## 📝 Git Commit Guidelines

Write clean, descriptive commit messages following Conventional Commits format:

```text
<type>(<scope>): <short summary>

[optional body]

[optional issue reference]
```

### Commit Types:
- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation changes
- `style`: Formatting, missing semi-colons, no code changes
- `refactor`: Refactoring code without changing functionality
- `perf`: Code changes that improve performance
- `test`: Adding or updating tests

### Example:
```text
feat(overlay): add spotlight focus mode tool

Implemented a circular spotlight overlay component for high-visibility presentations.
Closes #42
```

---

## 🔄 Pull Request Process

1. Fill out the **Pull Request Template** completely.
2. Ensure your code passes all lint checks and compiles cleanly without warnings or errors.
3. Ensure feature changes do not degrade overlay drawing responsiveness or battery life.
4. Maintain backward compatibility with supported Android OS versions (Android 7.0+).
5. Request a review from the maintainers.
6. Address any feedback prompt and respectfully.

---

## 🎨 Code Style & Best Practices

- **Clean Architecture:** Keep UI overlay logic separate from drawing canvas mathematical rendering.
- **Resource Management:** Ensure bitmap canvas instances and paint resources are recycled properly to prevent memory leaks.
- **Permission Safety:** Always verify overlay permission (`Settings.canDrawOverlays`) before launching floating window services.
- **Comments & Documentation:** Write clear comments for non-trivial mathematical calculations (e.g., laser path fading, smooth bezier curve calculations).

---

## 📄 License

By contributing, you agree that your contributions will be licensed under the project's [MIT License](LICENSE).
