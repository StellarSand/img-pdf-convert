# img-pdf-convert

**img-pdf-convert** tool allows you to convert images to PDF files and vice versa on GNU/Linux, macOS and Windows systems.



## Contents
- [Supported OS](#supported-os)
- [Prerequisites](#prerequisites)
- [Supported image formats for converting to PDF](#supported-image-formats-for-converting-to-pdf)
- [Installation](#installation)
- [Available options](#available-options)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)



## Supported OS
- GNU/Linux
- Windows
- macOS



## Prerequisites
- [Python3](https://www.python.org/downloads/)
- [Pillow](https://pypi.org/project/Pillow/): Install using `pip install Pillow`
- [pdf2image](https://pypi.org/project/pdf2image/): Install using `pip install pdf2image`



## Supported image formats for converting to PDF
- JPEG
- PNG
- WEBP
- TIFF
- BMP
- ICO
- ICNS
- PBM
- PGM
- PPM



## Installation
**1. Clone this repo:**
```
git clone https://github.com/StellarSand/img-pdf-convert.git
```

**2. Move into the project directory:**
```
cd img-pdf-convert
```

**3. Give executable permissions to the script (Not required for Windows):**
```
chmod +x img-pdf-convert
```



## Available options:
```
-h, --help              Show this help message and exit
-lf, --list-formats     Show a list of supported image formats

---Image(s) to PDF---
-i, --image-files       Path to the image files
-o, --output-file       Output file

---PDF(s) to image(s)---
-p, --pdf-files         Path to the PDF files
-d, --directory         Output directory for extracted images (optional)
-if, --image-format     Output format for extracted images (optional, default: jpeg)
```



## Usage
```
python3 img-pdf-convert -i <image> -o <output file>
```

```
python3 img-pdf-convert -p <PDF>
```

**Examples:**
```
python3 img-pdf-convert -i icon.png -o icon.pdf
```

```
python3 img-pdf-convert -i icon1.png icon2.jpg -o /home/user/Downloads/new_icon.pdf
```

```
python3 img-pdf-convert -p document.pdf
```

```
python3 img-pdf-convert -p document1.pdf document2.pdf -d /home/user/Downloads -if png
```

**Convert all images with a specified format to PDF file:**
```
python3 img-pdf-convert -i *.png *.jpg -o icon.pdf
```

**Convert all PDF files to images:**
```
python3 img-pdf-convert -p *.pdf
```



## Contributing
Pull requests can be submitted [here](https://github.com/StellarSand/img-pdf-convert/pulls).



## License
This project is licensed under the terms of [GPLv3 license](https://github.com/StellarSand/img-pdf-convert/blob/main/LICENSE).
