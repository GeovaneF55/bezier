Instalação & Execução

Método para funcionamento no Ubuntu:

Primeiro é preciso instalar o gerenciador de pacotes do python o PIP:

$ sudo apt update
$ sudo apt install python3-pip

Logo após a instalação do PIP, clonar o repositório no diretório de trabalho:

$ sudo apt update
$ sudo apt install git
$ git clone https://github.com/GeovaneF55/bezier.git [caminho/para/repositorio]

Será necessário, em seguida, navegar até a pasta raíz do projeto e instalar as dependências necessárias para a execução do programa (numpy, pyqt5):

$ cd caminho/para/repositório/bezier
$ sudo pip3 install -e .

Ao instalar as dependências e estando dentro da pasta raíz do projeto, vá para a pasta bezier e lá execute:

$ python3 bezier.py

Como Utilizar (Manual do Usuário):

No menu superior temos os seguintes botões:

    1. Arquivo

    • Curvas Paramétricas de Bêzier: Ao clicar você poderá definir 4 pontos como parâmetros para a curva de Bêzier que será plotada logo em seguida.
    • Limpar: Ao clicar em limpar a curva de Bêzier aparente na tela será apagada.
    • Sair: Ao clicar em sair, o programa terminará

    2. Ver

    • Ver Barra de Status: Habilita/Desabilita a barra de status do programa na parte inferior do programa

Na  Toolbar superior temos os mesmos botões do menu superior do grupo de Arquivo

Organização do Código:

O Código contém as seguintes classes:

    • Drawer
    • MyWidget
    • MyPaint

O algorítmo de Bêzier foi implementado pelo metodo de mesmo nome e foi utilizado os cálculos da matriz de bêzier para descobrir os valores constantes da função que define a curva.
