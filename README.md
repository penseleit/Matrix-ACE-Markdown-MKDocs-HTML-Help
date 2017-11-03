# Matrix ACE Web Help

This is the repo for the web help of Matrix ACE.

Documentation is written in Markdown, and [MKDocs](http://www.mkdocs.org/) is used to generate static html content as output documentation.

The theme [Material](https://squidfunk.github.io/mkdocs-material/) for MKDocs is used to give the output its look and feel.

The Markdown used is [Python Markdown](https://pythonhosted.org/Markdown/), based on [John Gruber's Markdown](https://daringfireball.net/projects/markdown/syntax)

## Building the documentation
### Setup
1. Install Python onto your computer
2. Ensure you also have `pip` (the Python Package Manager) installed
3. Open a command prompt and type:

        $python --version
        #Python 3.5.0

        $pip --version
        #pip 9.0.1

1. If Pip is not installed, at the command prompt type:

        $python get-pip.py

1. At the command prompt, install the MKDocs and Material theme Python packages:

        $pip install mkdocs mkdocs-material

1. Check that it all installed:

        $mkdocs --version
        #mkdocs version 0.17.1

1. Download the Matrix ACE Help source files to a folder on your computer, e.g: `C:\src\Matrix ACE Help`
2. At the command prompt, naviagte the the folder where you downloaded the Matrix ACE source files

        $cd c:\src\Matrix ACE Help

1. At the command prompt, type the `serve` command to start the MKDocs in-built webserver:

        $mkdocs serve

1. By default, the MKDocs web server serves its pages to 127.0.0.1:8000
2. Open a web browser and type in http://127.0.0.1:8000 to see the contents of the Matrix ACE source folder displayed
3. To build the static html output, type:

        $mkdocs build

1. The output is built in the `site` folder:  `C:\src\Matrix ACE Help\site`

## Deploying the documentation
The content of the `site` folder is used as the docuemntation for the Matrix ACE product.
Copy the contents of this folder for use in the installation package for the product.
