[![Electron](https://img.shields.io/badge/Built%20With-Electron-47848F?logo=electron&logoColor=white)](https://www.electronjs.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Platform](https://img.shields.io/badge/Cross--Platform-Windows%20%7C%20macOS%20%7C%20Linux-4ea94b?logo=windows&logoColor=white)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

# 📝 Electron Markdown Editor ![Electron Markdown Editor Logo](https://skillicons.dev/icons?i=electron)

*A lightweight, cross-platform desktop application for creating and managing Markdown notes.*

---

## 🚀 Features

- 📝 **Markdown Support:** Write and preview Markdown notes seamlessly.
- 💻 **Cross-Platform:** Works on Windows, macOS, and Linux.
- 🧘 **Simple Interface:** Focus on productivity with a clean and intuitive UI.
- 🪄 **Live Preview:** See your Markdown rendered in real-time.
- 📁 **File Management:** Save, load, and organize your notes easily.

---

## 🛠️ How It Works

### ⚡ Installation

**环境要求：** Node.js ≥ 18（本项目在 Node v22.22.2 + npm 10.9.7 环境下测试通过）

1. 🌀 **Clone the repository:**
   ```bash
   git clone https://github.com/yinxi5524-eng/electron-markdown-editor.git
   ```

2. 📁 **Navigate to the project directory:**
   ```bash
   cd electron-markdown-editor
   ```   

3. 📦 **Install dependencies:**
   ```bash
   npm install
   ```
   > 💡 国内网络提示：如果 Electron 二进制下载超时，可使用镜像：
   > ```bash
   > ELECTRON_MIRROR="https://registry.npmmirror.com/-/binary/electron/" npm install --registry https://registry.npmmirror.com
   > ```

4. ▶️ **Start the application:**
   ```bash
   npm start
   ```

**依赖清单（package.json）：**

| 依赖 | 类型 | 版本 | 用途 |
|---|---|---|---|
| electron | devDependencies | ^33.0.0 | 桌面应用运行时 |
| electron-builder | devDependencies | ^25.1.8 | 打包生成 Windows 安装包 |

> 📌 原仓库 package.json 中 electron 版本写作 `^latest`，npm 不接受该写法（`npm install` 会报 `EINVALIDTAGNAME` 错误），本 Fork 已修正为 `^33.0.0`。

---

## 🧑‍💻 Usage

- 🗂️ Open the application.
- 🆕 Create a new Markdown file or load an existing one.
- ✍️ Write your notes in the editor pane.
- 👀 View the **live preview** of your Markdown in the preview pane.
- 💾 Save your notes locally for future use.

---

## 📂 Project Structure

```text
electron-markdown-editor/
├── src/                # 🛠️ Source code for the application
├── assets/             # 🖼️ Images, icons, and other assets
├── package.json        # 📦 Project dependencies and scripts
├── README.md           # 📄 Project documentation
└── main.js             # ⚙️ Electron main process
```

---

## 📸 Screenshots

### ✏️ Editor Interface
![Editor Screenshot](assets/image2.png)

### 👓 Live Preview
![Preview Screenshot](assets/image1.png)

---

## 🤝 Contributing

Contributions are welcome!  
Feel free to open issues or submit pull requests to improve the project.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

🤝 Contributing
Contributions are welcome!
Feel free to open issues or submit pull requests to improve the project.
