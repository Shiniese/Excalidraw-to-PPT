# **Excalidraw-to-PPT**

![Python](https://img.shields.io/badge/python-3.12-blue) ![License](https://img.shields.io/badge/license-MIT-green)

中文文档请访问：[中文文档](#chinese-documentation)

一个将 Excalidraw (.excalidraw) 文件转换为 PowerPoint（PPT）演示文稿的 Python 工具。它从 `.excalidraw` 文件中提取嵌入的图像，将其保存为 PNG 格式，并组织到整齐排版的 PowerPoint 幻灯片中。

---

## **功能**
- 自动从 `.excalidraw` 文件提取 base64 编码的图像。
- 将提取的图像作为单独的 PNG 文件保存到专用文件夹中。
- 生成一个将所有图像按网格布局排列的 PowerPoint 演示文稿。
- 支持单个目录中的多个 `.excalidraw` 文件。

---

## **安装**

1. **克隆存储库**
   ```bash
   git clone https://github.com/Shiniese/Excalidraw-to-PPT.git
   cd Excalidraw-to-PPT
   ```

2. **安装依赖项**
   使用 `pip` 安装所需的 Python 库：
   ```bash
   pip install python-pptx Pillow
   ```

3. **放置你的 Excalidraw 文件**
   将你的 `.excalidraw` 文件复制到项目目录中。

---

## **使用方法**

1. 运行脚本：
   ```bash
   python excalidraw_to_ppt.py
   ```

2. 该工具将会：
   - 从当前目录中所有 `.excalidraw` 文件提取图像。
   - 将图像保存到以每个文件命名的子文件夹中。
   - 生成包含这些图像的 PowerPoint 文件 (`excalidraw_to_ppt.pptx`)。

---

## **示例**

#### 输入：
你有三个 `.excalidraw` 文件：
- `diagram1.excalidraw`
- `diagram2.excalidraw`
- `notes.excalidraw`

#### 输出：
- `diagram1/` 文件夹中包含提取的图像（例如，`diagram1-1.png`, `diagram1-2.png`）。
- `diagram2/` 文件夹中包含提取的图像（例如，`diagram2-1.png`, `diagram2-2.png`）。
- `notes/` 文件夹中包含提取的图像（例如，`notes-1.png`）。

此外会生成一个 PowerPoint 文件 (`excalidraw_to_ppt.pptx`)，其中每张幻灯片对应一个 `.excalidraw` 文件，并整齐排列对应的图像。

---

## **依赖项**

需要以下 Python 库：
- `python-pptx`（用于创建 PowerPoint 演示文稿）
- `Pillow`（用于图像处理）
- `os` 和 `json`（Python 内置模块）

通过以下命令安装它们：
```bash
pip install python-pptx Pillow
```

---

## **贡献**

如果你想为该项目做出贡献：
1. Fork 存储库。
2. 创建新分支 (`git checkout -b feature/YourFeatureName`)。
3. 提交更改 (`git commit -m "添加某些功能"`)。
4. 推送到分支 (`git push origin feature/YourFeatureName`)。
5. 开启 Pull Request。

---

## **许可证**

该项目根据 **MIT 许可证**发布。详情请查看 [LICENSE](https://github.com/Shiniese/Excalidraw-to-PPT/blob/main/LICENSE) 文件。

---

## **致谢**

- 灵感来源于自动化设计工具与演示文稿之间的流程需求。
- 由 Python 库如 `python-pptx` 和 `Pillow` 提供支持。
