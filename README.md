
## Pré-Requisitos do Robot Framework
Para rodar o Robot Framework é necessário instalar as seguintes ferramentas:

- Instalar o [Python 3.x e o pip](https://www.python.org/downloads/).
Para o Linux Mint o python a principio vem instalado em uma versão 3.X mas o pip a principio não, para instalar o pip execute o seguinte comando:
```
sudo apt install python3-pip
```
para verificar se o python e o pip estão instalado execute:
```
pip --version ou pip3 --version
python3 --version

```
- Instalar o Robot Framework, no terminal execute o seguinte comando: 
```
pip install -U robotframework robot --version
```
- Instalar Selenium Library para o Robot Framework:
```
pip install --upgrade robotframework-seleniumlibrary
```
A biblioteca do Selenium requer um driver para fazer a interface com o navegador escolhido e que precisa ser instalado antes que o projeto possa ser executado. o driver também precisam estar no PATH do computador, por exemplo após fazer o download, colocar o arquivo em /usr/local/bin no caso do linux, para verificar o PATH basta executar ``` echo $PATH ``` no terminal do linux. abaixo está o link para os drivers (apenas um é necessário).
- [ChromeDriver](https://chromedriver.chromium.org/downloads) para o google chrome (necessário baixar o arquivo com a mesma versão do navegador).
- [GeckoDriver](https://github.com/mozilla/geckodriver/releases) para o firefox.

## Instruções para rodar o teste:
Para rodar o teste, após clonar o repositório e realizado os pré-requisitos, pode ser utilizado o seguinte comando no terminal, dentro da pasta suiteDeTestesExemplo:
```
robot -d ./results tests 
```
caso o GeckoDriver tiver sido selecionado, é necessário rodar o seguinte comando:
```
robot -d ./results -v BROWSER:firefox tests
```

## Links Importantes
- [Robot Framework](https://robotframework.org/#libraries)
- [Libraries RobotFramework](https://robotframework.org/#libraries)
- [Dicas](http://robotizandotestes.blogspot.com/)
- [Técnica BDD](https://www.primecontrol.com.br/bdd-e-muito-mais-do-que-casos-de-testes/)

