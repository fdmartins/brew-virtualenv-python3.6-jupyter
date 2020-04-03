# fdmartins
Criando Ambiente Virtual Python3.6 e macOS Catalina.
Estamos focando na versão 3.6.5_1 pois, até inicio de 2020, é a melhor versão compativel com opencv, keras, tensorflow e outras bibliotecas de machine learning.



### Verifique as versões atuais
```bash
brew info python
```
### Instalar Python 3.6.5
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


To install virtualenv via pip run:
```bash
pip3 install virtualenv
```

Se aparece erros como:'SSLError("Can't connect to HTTPS URL because the SSL module is not available.", sera necessario executar o comando abaixo e repetir todo processo de insalação acima.

```bash
brew update && brew upgrade
brew uninstall --ignore-dependencies openssl
brew install https://github.com/tebelorg/Tump/releases/download/v1.0.0/openssl.rb
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
#### Instalar Jupyter Notebook

```bash
pip install jupyterlab
```

##### Executar Jupyter Notebook
```bash
jupyter notebook
```
