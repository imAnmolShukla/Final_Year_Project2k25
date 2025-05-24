# Malware Binary to Grayscale Image Converter 🦠🖼️

This project converts malware binary files into grayscale images for use in machine learning and computer vision-based malware classification systems.

## 📌 Overview

Malware binaries often contain patterns that are visually detectable when converted to images. This script reads binary files, reshapes them into grayscale images, and saves them in a format suitable for CNN-based models.

## 🛠️ Features

- Automatically extracts malware samples from a `.zip` archive.
- Dynamically chooses image width based on file size.
- Converts each binary into a padded 2D grayscale image.
- Saves output images in a dedicated folder with informative filenames.

## 🗂️ Output

The script saves images in a folder named `malware_images/`, where each image is named like:
```

virus\_sample\_128w\.png
trojan\_file\_256w\.png

````
The suffix (e.g., `128w`) indicates the image width.

## 🚀 How to Run

1. Place your malware binaries in a ZIP file (e.g., `malware_binaries.zip`).
2. Run the script:

```bash
python generate_malware_images.py
````

3. Check the `malware_images/` folder for the output.

## 🧠 Why This Helps

This technique is useful in:

* Malware classification using CNNs
* Visual pattern recognition in binaries
* Dataset preparation for malware detection ML models

## ⚠️ Disclaimer

* **Do not execute any binary files.**
* Handle malware samples in a **secure, sandboxed environment**.
* Use only for **educational or research** purposes.
