# How to learn modern Python
**A guide to the adventurer**<br>
<br>
[Click para versão em Português/Portuguese version](./README_Portugues.md)  <br>
<br>
First to learn modern Python you have to choose an operating system. The Python is the same in all of them but some settings and the libs used by your future programs may be supported in one OS and not in the other OS. In this guide I focus on the development in Linux and Windows, but the info can also be useful for other operating systems. <br>

* In this context we start by installing Ubuntu Linux, as a stand alone machine or as a virtual machine. If you plan to use Windows jump this step. <br>
[Ubuntu](https://www.ubuntu.com/download/desktop) <br>

* Install the Python distribution Anaconda, with Python version 3.7 or greater. <br>
[Anaconda Distribution](https://www.anaconda.com/distribution/)

* Install an IDE (Integrated Development Environment) and an editor, I choose Visual Studio Code to develop but I also like to have Sublime Text to open a file quickly. Both work on Linux, Windows and Mac, and both are fast. <br>
[Visual Studio Code](https://code.visualstudio.com/) <br>
[Sublime Text](https://www.sublimetext.com/) <br>

* In youtube search and see some videos on how to use Visual Studio Code and explore the menus and buttons.

* In Visual Studio Code, install the following Plugins directly in the IDE (Square button on the left): <br>
[Python ... syntax highlighting, code completion and debugging](https://marketplace.visualstudio.com/items?itemName=ms-python.python) <br>
[Anaconda Extension Pack ... ](https://marketplace.visualstudio.com/items?itemName=ms-python.anaconda-extension-pack) <br>
[Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) <br>
[Code Spell Checker... comments and code](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) <br>
[Markdown All in One ... markdown syntax highlighting and preview](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) <br>
[Better Comments ... TODO list's in code comments and more](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments) <br>

* Create a new directory for the project ex: proj/test_01_proj, create a Python file with extension ".py", ex: test_01.py and write "print("Hello World!")".

* Create and setup the virtual environment and the packages in Anaconda for the project on Linux or Windows. This will means that the packages you install will be installed specifically for your project virtual environment an not for the base installation.<br>

See the conda version:

```
    $ conda -V
```

Update conda

```
    $ conda update conda
```

Create a virtual environment for your project (substitute yourenvname by the name of the environment ex: test_01_proj and the x.x by 3.7 the version of Python in the future environment).

```
    $ conda create -n yourenvname python=x.x anaconda
    ex: $ conda create -n test_01_proj python=3.7 anaconda
```

See the environments that were created.

```
    $ conda info -e
```

To activate the environment

```
    $ source activate yourenvname
    ex: $ source activate test_01_proj
```

or

```
    $ conda activate test_01_proj
```

To desactivate an active environment

```
    $ source activate yourenvname
    ex: $ source desactivate
```

or

```
    $ conda deactivate
```

Install additional Python packages to a virtual environment.

```
    $ conda install -n yourenvname [package]
    ex: $ conda install -n test_01_proj svgwrite
```

Delete a no longer needed virtual environment <br>

```
    $ conda remove -n yourenvname -all
    ex: $ conda remove -n test_01_proj -all
```

* In your project select the correct interpreter.<br>
ctrl + shift + p then write "Python select interpreter" command and choose the virtual environment test01_proj that you created from the drop-down selection.   

* Install in Python PyLint and CTags on the virtual environment.

```
    $ conda install -n test_01_proj -c conda-forge pylint
    $ conda install -n test_01_proj -c conda-forge ctags
```

* In Visual Studio Code, copy one ".env" file from inside GitHub to the directory of the project, it will initialize the environment variables, adjust the paths to your virtual environment (user). The following is necessary for now because VSCode doesn't activate automatically the virtual environment when debugging.<br>
For Windows copy the file ".env" in github to your project directory. <br>
For Linux copy the file ".env_linux" in github to your project directory and rename it ".env". 

* Now for Python it self. View two times the following 45 minutes video that explains the main parts of the Python language. View it from the beginning to the end, even if you don’t understand all of what is explained. In the next step the Python language will be explained in more detail. Ignore the part of the video that teach how to install Python and the IDE PyCharm. <br> 
[Python Programming video by Derek Banas](https://www.youtube.com/watch?v=N4mEzFDjqtA)  

* Follow the free official tutorial of Python and study it well. <br>
[The Python Tutorial](https://docs.python.org/3/tutorial/) 

* Read the following book from cover to cover, don't look at the title see the table of contents it's a really good Python all around book. <br>
[Effective Computation in Physics: Field Guide to Research with Python 1st Ed. by Anthony Scopatz, Kathryn D. Huff](https://www.amazon.com/Effective-Computation-Physics-Research-Python-ebook/dp/B010ORQ8DG/ref=sr_1_10)

* You only really understand a programming language and programming generally, after you have sean many projects written in the language. So study the following book full of projects and the respective code. <br>
[Python Playground: Geeky Projects for the Curious Programmer 1st Ed by Mahesh Venkitachalam](https://www.amazon.com/Python-Playground-Projects-Curious-Programmer-ebook/dp/B017AH8H7I/ref=pd_sim_351_6/175-5456264-3791003) 

* For all your Python development your main source of documentation will always be <br>
[Python 3.x documentation](https://docs.python.org/3/)

* **Jupyter Notebooks** <br>
  [1. Introduction - Jupyter Tutorial](https://www.youtube.com/watch?v=Rc4JQWowG5I&list=PL1m-6MPBNAZfF-El7BzqaOrCrTBRgH1Nk&index=1) <br>
  [2. Markdown & LaTeX - Jupyter Tutorial](https://www.youtube.com/watch?v=-F4WS8o-G2A&list=PL1m-6MPBNAZfF-El7BzqaOrCrTBRgH1Nk&index=4) <br>
  [3. Python 3 - Jupyter Tutorial](https://www.youtube.com/watch?v=1I2Bz0qbMsc&list=PL1m-6MPBNAZfF-El7BzqaOrCrTBRgH1Nk&index=5) <br>
  [4. Numpy - Jupyter Tutorial](https://www.youtube.com/watch?v=ZABbRR0tfuc&list=PL1m-6MPBNAZfF-El7BzqaOrCrTBRgH1Nk&index=6)


If you do all this steps you will have a fair knowledge of Python and can start doing some cool projects in Python. <br>

Have fun! <br> 

Best regards,<br>
Joao Nuno Carvalho




