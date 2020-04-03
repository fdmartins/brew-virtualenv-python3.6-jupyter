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

execute o comando abaixo para ver se a versão do python3 é a que você precisa:
```bash
python3 --version
```
python 3.6.5_1


##### Installation
To install virtualenv via pip run:
```bash
pip3 install virtualenv
```

##### Usage
Creation of virtualenv.
Aqui usamos o nome machinelearning.
```bash
virtualenv -p python3 ~/.virtualenvs/machinelearning
```

Activate the virtualenv:
```bash
workon machinelearning
```

Deactivate the virtualenv:
```bash
deactivate
```

