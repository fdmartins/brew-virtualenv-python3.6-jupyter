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


Execute o pip3 e veja se não aparece erros como:'SSLError("Can't connect to HTTPS URL because the SSL module is not available.", se sim, sera necessario executar o comando abaixo e repetir o processo acima.

```bash
brew update && brew upgrade
brew uninstall --ignore-dependencies openssl
brew install https://github.com/tebelorg/Tump/releases/download/v1.0.0/openssl.rb
```


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

Verique se a versão do python dentro do ambiente virtual esta correta.
```bash
python --version
```

Para sair do virtualenv:
```bash
deactivate
```
##### Instalar Jupyter Notebook

```bash
pip install jupyterlab
```

##### Executar Jupyter Notebook
```bash
jupyter notebook
```
