![GitHub release (latest by date)](https://img.shields.io/github/v/release/ImageProcessing-ElectronicPublications/pdfcook)
![GitHub Release Date](https://img.shields.io/github/release-date/ImageProcessing-ElectronicPublications/pdfcook)
![GitHub repo size](https://img.shields.io/github/repo-size/ImageProcessing-ElectronicPublications/pdfcook)
![GitHub all releases](https://img.shields.io/github/downloads/ImageProcessing-ElectronicPublications/pdfcook/total)
![GitHub](https://img.shields.io/github/license/ImageProcessing-ElectronicPublications/pdfcook)

# pdfcook
Preprinting preparation tool for PDF ebooks.  

### Build and Install
Enter project directory and type:
```sh
make -j4  
sudo make install  
```

### Features
* PDF v1.7 support  
* Join or Split PDFs  
* Scale to any paper size, with specified margin  
* Write Page numbers  
* Write text  
* Transform pages (rotate, flip, move)  
* Booklet format arrange  
* 2 or 4 pages per page (2-up, 4-up)  

### Usage
See manual page (PDF or man page) for detailed usage  

Scale to print in A4 size paper  
```sh
pdfcook 'scaleto(a4)' input.pdf output.pdf  
```

Add binding margin after scaling (? for odd pages, + for even pages)  
```sh
pdfcook 'scaleto(a4) move(20){?} move(-20){+}' input.pdf output.pdf  
```

Add page numbers  
```sh
pdfcook 'number' input.pdf output.pdf  
```

Booklet format  
```sh
pdfcook 'book nup(2, paper=a4)' input.pdf output.pdf  
```

----

2021

