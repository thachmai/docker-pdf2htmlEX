pdf2htmlEX in a docker container
=================

Docker image for complied version of [pdf2htmlEX](http://coolwanglu.github.com/pdf2htmlEX/)

## Usage
To compile a PDF to HTML:

    sudo docker run -v "$PWD:/src" thachmai/pdf2htmlex <your_pdf_file> [other pdf2htmlex params...]

If you want to make it simpler for repeated use, you can define an alias for the above command, for example, in Ubuntu 14.04, you can do this:

    printf "\nalias pdf2html='sudo docker run -v \"$PWD:/src\" thachmai/pdf2htmlex'\n" >> ~/.bash_aliases

Then, simple run `pdf2html your_pdf` to compile a PDF.

## License
MIT

This is a fork of [Klokoy's](https://github.com/klokoy/pdf2htmlEX_docker) base image with some clean up and optimizations for ease of use.
