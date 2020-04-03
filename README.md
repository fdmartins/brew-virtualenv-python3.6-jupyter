# fdmartins
Criando Ambiente Virtual Python3.6 e macOS Catalina

#### Verifique as versões atuais
```bash
brew info python
```
### Para instalar a versão 3.6.5
Caso o comando acime não tenha a versão 3.6.5, instale executando:
```bash
brew unlink python

brew install --ignore-dependencies https://raw.githubusercontent.com/Homebrew/homebrew-core/f2a764ef944b1080be64bd88dca9a1d80130c558/Formula/python.rb

brew switch python 3.6.5_1

```

execute o comando abaixo para ver se a versão do python3 está a que você precisa:
```bash
python3 --version
```


##### Requirements
* Python 3
* Pip 3

```bash
$ brew install python3
```

Pip3 is installed with Python3

##### Installation
To install virtualenv via pip run:
```bash
$ pip3 install virtualenv
```

##### Usage
Creation of virtualenv:
```bash
$ virtualenv -p python3 <desired-path>
```

Activate the virtualenv:
```bash
$ source <desired-path>/bin/activate
```

Deactivate the virtualenv:
```bash
$ deactivate
```

