
build folder: this is used to build each ipynb file, and we can also test each ipynb file in this folder.

images: to save the images that the ipynb files need.

x.ipynb: each ipynb file represents a report for one specific trainning course.

x.html: this html can be read by the browser, and it can be created by running this command.
$ jupyter nbconvert --to html --template pj vina.ipynb # we need to install the pj template, see https://github.com/JanPalasek/pretty-jupyter.

