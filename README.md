# newpaper

Command line tool to organize and take notes for papers.

## Installation

1. Clone the repository to your local machine.
2. Add the path of `newpaper` to your `PATH` environment variable.
   e.g. add `export PATH="path-to-folder/newpaper:$PATH"` to your `.zshrc` file.
3. Make a new directory for where you want to store your papers and notes.
4. (Optional) Make a file in said folder called `ledger` (with no extension). 
   This will keep track of the papers which are already stored.

## Usage

Go to the directory for which you want to store your papers and notes.

For taking notes of arxiv papers, simply copy the arxiv id of said paper, e.g. `1205.1735v4` and run the command 
`newpaper Name-of-folder 1205.1735v4` 
This will create a new directory with the name `Name-of-folder` and download the paper in that folder.
Moreover, it will create a new TeX file `Name-of-folderrm.tex` which copies the template TeX file while replacing 
the title and subtitle with the title of the paper and the arxiv link respectively.

For general pdfs, the command works similarly with the only difference being that you should replace 
the arxiv id with the link to the pdf.

Using the command in the directory where you have the `ledger` file will record the id into the `ledger` and 
future uses in said directory will check whether or not the id is already in the `ledger`.
