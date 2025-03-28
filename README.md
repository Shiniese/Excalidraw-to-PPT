# **Excalidraw-to-PPT**

![Python](https://img.shields.io/badge/python-3.12-blue) ![License](https://img.shields.io/badge/license-MIT-green)

For Chinese documentation, please visit: [中文文档](https://github.com/Shiniese/Excalidraw-to-PPT/blob/main/README_zh.md)

A Python tool that automates the process of converting Excalidraw (.excalidraw) files into PowerPoint presentations (PPT). It extracts embedded images from the `.excalidraw` file, saves them as PNGs, and organizes them into a neatly formatted PowerPoint slide.

---

## **Features**
- Automatically extract base64-encoded images from `.excalidraw` files.
- Save extracted images as individual PNG files in a dedicated folder.
- Generate a PowerPoint presentation with all images arranged in a grid layout.
- Support for multiple `.excalidraw` files in a single directory.

---

## **Installation**

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Shiniese/Excalidraw-to-PPT.git
   cd Excalidraw-to-PPT
   ```

2. **Install Dependencies**
   Install the required Python libraries using `pip`:
   ```bash
   pip install python-pptx Pillow
   ```

3. **Place Your Excalidraw Files**
   Copy your `.excalidraw` files into the project directory.

---

## **Usage**

1. Run the script:
   ```bash
   python excalidraw_to_ppt.py
   ```

2. The tool will:
   - Extract images from all `.excalidraw` files in the current directory.
   - Save the images into subfolders named after each file.
   - Generate a PowerPoint file (`excalidraw_to_ppt.pptx`) containing the images.

---

## **Example**

#### Input:
You have three `.excalidraw` files:
- `diagram1.excalidraw`
- `diagram2.excalidraw`
- `notes.excalidraw`

#### Output:
- `diagram1/` folder with extracted images (e.g., `diagram1-1.png`, `diagram1-2.png`).
- `diagram2/` folder with extracted images (e.g., `diagram2-1.png`, `diagram2-2.png`).
- `notes/` folder with extracted images (e.g., `notes-1.png`).

A PowerPoint file (`excalidraw_to_ppt.pptx`) will be created, containing slides for each `.excalidraw` file with corresponding images arranged neatly.

---

## **Dependencies**

The following Python libraries are required:
- `python-pptx` (for creating PowerPoint presentations)
- `Pillow` (for image processing)
- `os` and `json` (built-in Python modules)

Install them using:
```bash
pip install python-pptx Pillow
```

---

## **Contributing**

If you'd like to contribute to this project:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeatureName`).
3. Commit your changes (`git commit -m "Add some feature"`).
4. Push to the branch (`git push origin feature/YourFeatureName`).
5. Open a pull request.

---

## **License**

This project is licensed under the **MIT License**. See the [LICENSE](https://github.com/Shiniese/Excalidraw-to-PPT/blob/main/LICENSE) file for details.

---

## **Credits**

- Inspired by the need to automate workflows between design tools and presentations.
- Powered by Python libraries like `python-pptx` and `Pillow`.
