[![Electron](https://img.shields.io/badge/Built%20With-Electron-47848F?logo=electron&logoColor=white)](https://www.electronjs.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Platform](https://img.shields.io/badge/Cross--Platform-Windows%20%7C%20macOS%20%7C%20Linux-4ea94b?logo=windows&logoColor=white)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

# 📝 2026年底的风吹来一个markdown编辑器

*A lightweight, cross-platform desktop application for creating and managing Markdown notes.*

> 本仓库是课程作业项目：Fork 自 [Achintha-999/electron-markdown-editor](https://github.com/Achintha-999/electron-markdown-editor)，在此基础上完成了应用名修改、界面文案中文化、主题色更换与打包发布。

## 🎨 我的改动（vs 原版）

| 改动项 | 原版 | 改造后 |
|---|---|---|
| 应用名 | Markdown Notes | 2026年底的风吹来一个markdown编辑器 |
| 界面语言 | 英文（New/Open/Save…） | 中文（新建/打开/保存…） |
| 主题色 | 深蓝 #2c3e50 + 蓝 #3498db | 深青绿 #1e3a35 + 青绿 #16a085 |
| 弹窗文案 | 英文（Unsaved Changes…） | 中文（未保存的更改…） |
| 修复 | electron 版本写作 `^latest`（npm 无法安装） | 修正为 `^33.0.0`，补充 electron-builder 打包配置 |

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

## 📦 构建与打包（Windows）

打包使用 [electron-builder](https://www.electron.build/)，配置位于 `package.json` 的 `build` 字段。

```bash
# 1. 安装依赖（含 electron-builder）
npm install

# 2. 打包 Windows 安装包（NSIS 安装程序 + 便携版 exe）
npm run dist
```

**产物说明**（输出在 `dist/` 目录）：

| 文件 | 类型 | 说明 |
|---|---|---|
| `*. Setup.exe` | NSIS 安装包 | 双击安装，可选安装目录 |
| `*.exe`（portable） | 便携版 | 免安装直接运行 |

> 💡 国内网络提示：electron-builder 下载 Electron 打包底包较慢或超时时，设置镜像：
> ```bash
> ELECTRON_MIRROR="https://registry.npmmirror.com/-/binary/electron/" npm run dist
> ```

**注意**：`dist/`、`*.exe` 等构建产物已被 `.gitignore` 排除，不进入仓库，仅通过 GitHub Releases 分发。

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
