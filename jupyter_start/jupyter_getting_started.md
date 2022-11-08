# Jupyter notebooks to organize and annotate python

Jupyter notebooks offer an environment where you can write, run, and annotate python code using code boxes that can be specified as either markdown or python. It is ideal for providing descriptions or annotations of code in easily readable markdown


## Installing Jupyter

Jupyter is an independent software for writing and executing python and markdown code. Before you can get started writing, running and displaying code and markdown text using Jupyter notebooks, you will need to install the software. Below are a few ways to approach this.


I. If you prefer command line access and opening files from the command line, you can easily install `Jupyter` using `pip`, `brew`, or `conda`. 

Install with `pip` (installation tool built into python).

    $ pip install jupyter

Once `Jupyter` is installed, you can open a new notebook from anywhere with:

    $ jupyter-notebook

You can click the `new` button on the top right of this window, and select `python3` to open an untitled workbook in the current working directory. You can save this file as whatever you like (in the current working directory) by clicking on `save as` under the `file` menu.

To open an already existing `Jupyter Notebook` from the command line, follow the example below. Note that the file extension for `Jupyter Notebook` files is `.ipynb`.

    $ jupyter-notebook logger_jupyter.ipynb

Once you do that, the specified file with open in `Jupyter`


![My Image](images/jupyter_file.png)

II. Many of you have already installed the Anaconda Navigator suite of GUI applications. You can start Jupyter from the `Jupyter Notebook` icon in the application menu. 

![My Image](images/navigator_menu.png)

Once you do that, a `Jupyter` server will launch on your screen that will display Jupyter in an html viewer within your default web browser. Note that this is not a connection to an internet site, but an interactive html based application. From here you can navigate your directory tree to open an already existing `Jupyter Notebook` or can click on `new` to create a new file. The menu bar at the top should be largely self explanatory and self explorable.

![My Image](images/jupyter_menu.png)


Once you open a new `Jupyter Notebook` it will display a menu at the top and a blank box with a cursor. There is a drop down menu on the right where you can switch between code and markdown to control how you what you type in each box is interpretted, shown in the image below. 

![My Image](images/code_md_menu.png)



## Writing markdown in code boxes

Markdown is a simple markup language for creating formatted text using a plain-text editor that renders into simple and easily readable formatted html. Markdown is widely used software documentation pages, readme files, and is the languate used to write the primers I have created for this course. 


Due to its simplicity, markdown is very effective for annotating and describing python code. You can keep it as simple as just writing in plain text, or you can use more detailed formatting, including different font sizes for headers and subheaders, bulleted lists, code boxes to demo commands, and font formatting such as bold and italics.

To write markdown in a jupyter code block, start by selecting markdown from the dropdown menu on the upper right. Then type whatever you intend into the code box. The image below shows an example of what raw markdown looks like for several features it enables.

![My Image](images/markdown_raw.png)

To process, or render, the markdown into how it should appear in html, click the `run` button on the top menu. The raw markdown above will be processed into html as below.

![My Image](images/rendered_markdown.png)


## Writing python in `Jupyter`

There is little explanation needed here. Just select python3 from the code selection menu when you highlight a new code box, and proceed to write python code. Once you run the code boxes, the python code will be processed. If there is stdout, it will be printed below the code box. Image below shows some simple examples.

![My Image](images/alternating_boxes.png)

There are limitations here, in that loops must be fully contained within a single code box. So if you have a set of four nested loops, they can not be interrupted by boxes of markdown, or separate boxes of python.

Variables generated and stored in previous code boxes, however, are available in subsequent code boxes, so be conscentious of scope. For the most part, you should learn quickly that using `Jupyter Notebooks` is a pretty easy way to write organized python code.

## Exporting from `Jupyter`

There are options for exporting and downloading different types of files from `Jupyter`. The `download as` option under the `file` tab lists a menu of options. 

![My Image](images/download_as_menu.png)

If you download as `.py`, this will generate a text file that is a pythong script. Code and markdown text will be identical, but the markdown boxes will all be converted to comment lines.

![My Image](images/download_as_py.png)

Downloading as html or pdf is a convenient manner to generate uneditable documents that you can share with others to demo your code, or to share a full on tutorial or workflow.

![My Image](images/jupyter_html.png)



## 