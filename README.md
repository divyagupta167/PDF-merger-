PDF Merger Using pdf-merger-js
This repository contains a Node.js script that allows you to merge multiple PDF files into a single PDF using the pdf-merger-js library. The script provides a convenient way to merge entire PDFs or specific pages from different PDF files.

Getting Started
Clone this repository to your local machine.
Install the required dependencies by running npm install or yarn install.
Prerequisites
To use this script, you need to have Node.js installed on your machine.

How to Use
The main functionality is implemented in the mergePdfs function, which is exported from the pdfMerger.js file. The function takes two PDF file paths as input and merges them into a new PDF file.

Here's how to use the script:

Make sure you have the PDF files you want to merge available on your machine.
Require the mergePdfs function in your code and call it with the file paths as arguments.

Functionality
The mergePdfs function uses the pdf-merger-js library to merge the PDFs. It provides flexibility to choose whether to merge the entire PDFs or specific pages. The following functionalities are available:

Merge the entire PDFs: Pass the file paths of the PDFs you want to merge, and it will combine all the pages from both PDFs into a new PDF file.

Merge specific pages from a PDF: You can also merge only specific pages from a PDF by providing the desired page numbers or ranges when calling the merger.add() method. However, for the current implementation, only merging the entire PDFs and merging the second page of the second PDF are demonstrated in the provided code.

Saving the Merged PDF
The merged PDF is saved in the public directory with a filename based on the current timestamp. The PDF file will be named as <timestamp>.pdf.

Notes
The script is designed to run on Node.js and is not intended for browser use.
