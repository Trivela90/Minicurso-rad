# Source directory setup

**TODO**

# Setup at Ubuntu 20.04 LTS x64

## Environment setup

Instale o Git utilizando o seguinte link:
- https://git-scm.com/downloads

Instale o Python utilizando o seguinde link:
- https://docs.conda.io/en/latest/miniconda.html

Para utilizar o profile Miniconda, é necessário:
- Abrir a barra de comandos (Crtl+Shift+P), procurar por `>Preferences: Open Default Settings (JSON)` e selecioná-la;
- Em seguida, usar o comando (Crtl+F) para pesquisar profiles.windows;
- Copie o código referente ao "terminal.integrated.profiles.windows";
- Novamente, abrir a barra de comandos (Crtl+Shift+P), digitar `>Preferences: Open Settings (JSON)` e selecionar essa opção;
- Nessa aba, chamada "settings.json", cole o código que você havia copiado anteriormente;
- Retire "PowerShell":{} e "GitBash":{};
- Renomeie **Command Prompt** para **Command Prompt (Anaconda)**;
- Adicione o local completo do arquivo Anaconda Prompt (miniconda3), instalado em seu computador, no "args": [] da seguinte forma "args":["/K","local do activate.bat","local do miniconda3"];
- Defina o **Command Prompt (Anaconda)** ao inserir o comando `>Terminal: Select Default Profile` na barra de comandos (Crtl+Shift+P).


## Python setup

Para definir um ambiente virtual (ou virtual enviroment) para os pacotes do Python é necessário rodar esses comandos:

```bat
python -m venv venv
.\venv\Scripts\activate 
```

Para fazer a instalação dos pacotes, utilizaremos os seguintes comandos:

```bat
pip install -r dev-requirements.txt
```
Observação: se em seu prompt de comando a (base) for Develops_2, digite o commando `cd <caminho do Develops_2>\jupyter-template` para difinir a pasta "jupyter-template" como local padrão de trabalho.

## Jupyter setup

Make Jupyter venv **TODO**

# Setup at Windows 10

## Environment setup

Instale o git utilizando o seguinte link?
- https://git-scm.com/

Instale o python utilizando o seguinte link
- https://docs.conda.io/en/latest/miniconda.html

Para utilizar o profile do Miniconda
- Ir em configurações padrões (`>Preferences: Open Default Settings (JSON)`) e procurar por profiles.windows
- Copiar o trecho do profiles do **Command Prompt**
- Colar o trecho do profiles nas configurações "pessoais" (`>Preferences: Open Settings (JSON)`)
- Modificar o nome do profile para **Command Prompt (Anaconda)**
- Definir o profile padrão **Command Prompt (Anaconda)** através do comando `>Terminal: Select Default Profile`

## Python setup

Para definir um virtual enviroment para os pacotes do Python é necessário rodar esses comandos
```bat
python -m venv venv
.\venv\Scripts\activate
```

Para fazer as instalações dos pacotes, vamos utilizar os seguintes comandos:
```bat
pip install -r dev-requirements.txt
```


## Jupyter setup

Make Jupyter venv **TODO**
