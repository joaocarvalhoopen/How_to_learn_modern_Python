# Como aprender Python moderno
**Um guia para o aventureiro**<br>
<br>
[Click for the English version/Versão Inglesa](./README.md)  <br>
<br>
Em primeiro lugar para aprender Python moderno, temos de escolher o sistema operativo em que vamos desenvolver. A linguagem Python é a mesma em todos os sistemas operativos mas algumas configurações e as bibliotecas usadas pelos nossos futuros programas, podem existir para um S.O. e não existir para outro S.O. . Este guia foca no desenvolvimento em Linux e Windows, mas a informação poderá ser útil para outros sistemas operativos. <br>

* Neste contexto começamos por instalar a distribuição de Linux Ubuntu, como sistema operativo principal do PC ou como uma máquina virtual. Se tenciona usar Windows pode saltar este passo. <br>
[Ubuntu](https://www.ubuntu.com/download/desktop) <br>

* Instale a distribuição de Python Anaconda, com Python na versão maior ou igual a 3.7 . <br>
[Anaconda Distribution](https://www.anaconda.com/distribution/)

* Instale um IDE (Integrated Development Environment), ambiente de desenvolvimento integrado ou um editor de texto. Eu para desenvolver escolhi o Visual Studio Code, mas também gosto de ter instalado o editor Sublime Text para abrir ficheiros de forma rápida. Ambos funcionam em Linux, Windows e Mac, e ambos são rápidos e leves em termos de recursos. <br>
[Visual Studio Code](https://code.visualstudio.com/) <br>
[Sublime Text](https://www.sublimetext.com/) <br>

* Procure e veja no youtube, alguns vídeos sobre o Visual Studio Code e explore os menus e os botões. 

* Instale directamente no IDE do Visual Studio Code, os seguintes Plugins (Botão quadrado no lado esquerdo):<br>
[Python ... mostra a sintaxe em cores diferentes, completa o código e debugging](https://marketplace.visualstudio.com/items?itemName=ms-python.python) <br>
[Anaconda Extension Pack ... ](https://marketplace.visualstudio.com/items?itemName=ms-python.anaconda-extension-pack) <br>
[Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) <br>
[Code Spell Checker... comentários e código](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) <br>
[Markdown All in One ... markdown com sintaxe em cores diferentes e pré-visualização](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) <br>
[Better Comments ... Listas TODO nos comentários do código e outras extras](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments) <br>

* Crie uma directoria para o projecto ex: proj/test_01_proj, crie um ficheiro de Python com a extensão ".py", ex: test_01.py e escreva "print("Hello World!")".

* Criação e configuração do virtual environment (ambiente virtual) e dos packages (pacotes) em Anaconda para o projecto no Linux ou Windows. Isto significa que os pacotes que serão instalados serão somente instalados no ambiente virtual de Python usado no projecto e que não irão ser instalados na instalação base do Python.

Ver a versão do conda que está instalada:

```
    $ conda -V
```

Actualizar a versão do conda

```
    $ conda update conda
```

Crie um virtual environment (ambiente virtual) para o seu projecto (substitua yourenvname pelo nome do ambiente virtual ex: test_01_proj e o x.x por 3.7 , que será a versão do Python do seu futuro ambiente virtual).

```
    $ conda create -n yourenvname python=x.x anaconda 
    ex: $ conda create -n test_01_proj python=3.7 anaconda
```

Veja o ambiente que foi criado.

```
    $ conda info -e
```

Active o ambiente

```
    $ source activate yourenvname. 
    ex: $ source activate test_01_proj 
```

or

```
    $ conda activate test_01_proj
```


Para desactivar o ambiente.

```
    $ source activate yourenvname
    ex: $ source desactivate
```

or

```
    $ conda deactivate
```

Para instalar pacotes adicionais no seu ambiente virtual.

```
    $ conda install -n yourenvname [package]
    ex: $ conda install -n test_01_proj svgwrite
```

Para apagar um ambiente virtual que já não seja necessário.

```
    $ conda remove -n yourenvname -all 
    ex: $ conda remove -n test_01_proj -all 
```

* Dentro do Visual Studio Code, com o seu projecto aberto, seleccione o interpretador de Python usar neste projecto.<br>
ctrl + shift + p depois escreva o comando "Python select interpreter" e escolha o virtual environment test01_proj que acabou de criar, da caixa de selecção drop-down.   

* Instale os pacotes de Python, PyLint e CTags no ambiente virtual, eles serão usados para detectar os erros quando grava e para navegar entre os simbolos do código.

```
    $ conda install -n test_01_proj -c conda-forge pylint
    $ conda install -n test_01_proj -c conda-forge ctags
```

* No Visual Studio Code, copie o ficheiro ".env" que está dentro da directoria do projecto do GitHub. Este ficheiro vai inicializar as variáveis de ambiente na linha de comandos (shell), tem de ajustar os paths tendo em conta o seu user e o nome do seu ambiente virtual. É necessário fazer este passo pois o VSCode não activa automaticamente o ambiente virtual quando faz o debug.<br>
Para o Windows copie o ficheiro ".env" do github para a directoria do projecto. <br>
Para o Linux copie o ficheiro ".env_linux" do github para a directoria do projecto e renomei-o de ".env". 

* Agora em termos da linguagem Python propriamente dita. Vejam duas vezes o seguinte vídeo de 45 minutos a explicar a linguagem Python. Vejam do início até ao fim mesmo que não consigam perceber tudo o que é explicado. No passo seguinte a linguagem Python vai ser explicada mais com mais detalhe. Ignorem a parte da instalação do Python e do IDE PyCharm. <br>
[Python Programming video by Derek Banas](https://www.youtube.com/watch?v=N4mEzFDjqtA)  

* Leia atentamente o tutorial oficial do Python que é gratuito e é muito bom. Estude-o bem que vale a pena!  <br>
[The Python Tutorial](https://docs.python.org/3/tutorial/) 

* Leia o livro seguinte do início ao fim, não leve à letra o título do livro, veja o índex do livro. Este livro é um livro muito bom e muito abrangente que cobre várias áreas do desenvolvimento em Python. <br>
[Effective Computation in Physics: Field Guide to Research with Python 1st Ed. by Anthony Scopatz, Kathryn D. Huff](https://www.amazon.com/Effective-Computation-Physics-Research-Python-ebook/dp/B010ORQ8DG/ref=sr_1_10)

* Uma pessoa só percebe verdadeiramente uma linguagem de programação e a arte de programar, depois de ter visto e estudado vários projectos escritos na linguagem. Por isso peço-vos que estudem o livro seguinte que está cheio de pequenos projectos em várias áreas com o respectivo código em Python. <br>
[Python Playground: Geeky Projects for the Curious Programmer 1st Ed by Mahesh Venkitachalam](https://www.amazon.com/Python-Playground-Projects-Curious-Programmer-ebook/dp/B017AH8H7I/ref=pd_sim_351_6/175-5456264-3791003) 

* Para todo o desenvolvimento em Python a fonte principal de documentação será sempre o link seguinte para a documentação oficial <br>
[Python 3.x documentation](https://docs.python.org/3/)

* **Jupyter Notebooks** <br>
  [1. Introduction - Jupyter Tutorial](https://www.youtube.com/watch?v=Rc4JQWowG5I&list=PL1m-6MPBNAZfF-El7BzqaOrCrTBRgH1Nk&index=1) <br>
  [2. Markdown & LaTeX - Jupyter Tutorial](https://www.youtube.com/watch?v=-F4WS8o-G2A&list=PL1m-6MPBNAZfF-El7BzqaOrCrTBRgH1Nk&index=4) <br>
  [3. Python 3 - Jupyter Tutorial](https://www.youtube.com/watch?v=1I2Bz0qbMsc&list=PL1m-6MPBNAZfF-El7BzqaOrCrTBRgH1Nk&index=5) <br>
  [4. Numpy - Jupyter Tutorial](https://www.youtube.com/watch?v=ZABbRR0tfuc&list=PL1m-6MPBNAZfF-El7BzqaOrCrTBRgH1Nk&index=6)


Se fizer todos os passos anteriores, irá possuir um conhecimento bastante abrangente de Python e com isso poderá começar a fazer projectos muito interessantes e divertidos em Python. <br>

Espero que se divirta bastante com o Python!<br> 

Cumprimentos,<br>
Joao Nuno Carvalho




