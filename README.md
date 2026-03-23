# World Supervisor (Forge)

A simple Minecraft Forge mod for supervising and managing server/world behavior.

## ✨ Features

* Monitor server/world status
* Lightweight and server-friendly
* Designed for Forge-based environments

---

## 📦 Requirements

* Java 21
* Minecraft Forge
* Supported Minecraft versions depend on the build configuration

---

## 🚀 Build Instructions

### 🔧 Local Build

Clone the repository and run:

```bash
./gradlew build
```

After building, the `.jar` file will be generated in:

```
build/libs/
```

---

### 🤖 GitHub Actions (Recommended)

This project supports automatic builds via GitHub Actions.

#### How it works:

1. Push your code to the repository
2. Go to the **Actions** tab
3. Open the latest workflow run
4. Download the `.jar` file from **Artifacts**

---

## 🔁 Switching Minecraft Versions

This project uses a centralized configuration for version management.

### To change Minecraft version:

Edit:

```
gradle.properties
```

Example:

```properties
minecraft_version=1.21.10
forge_version=60.0.10
```

Then rebuild:

```bash
./gradlew build
```

---

## 🧩 Multi-Version Support (Optional)

You can build multiple Minecraft versions using GitHub Actions.

Example versions:

* 1.20.6
* 1.21.10

Each version will produce its own `.jar` file.

> Note: Some versions may require code changes due to Forge/Minecraft API differences.

---

## ⚠️ Compatibility Notes

* Not all Minecraft versions are fully compatible
* Major version upgrades (e.g. 1.20 → 1.21) may require code updates
* Always test the mod before deploying to production servers

---

## 📁 Project Structure

```
├── src/
├── build.gradle
├── gradle.properties
└── .github/workflows/
```

---

## 📜 License

MIT License (or your preferred license)

---

## 💡 Tips

* Always use `./gradlew` instead of system Gradle
* Use Java 21 for Minecraft 1.21+
* Check build logs if `.jar` is not generated

---

## 🤝 Contributing

Pull requests and issues are welcome!

---
