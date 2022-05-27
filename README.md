# ambiente-dev-linux

## Ubuntu

### Instalação Nodejs

<p align='center'>Para instalar uma versão expecífica do Node.js, você pode usar um PPA (arquivo de pacotes pessoal) mantido pelo NodeSource. Esses PPAs possuem mais versões do Node.js disponíveis do que os repositórios oficiais do Ubuntu. O Node.js v10, v12, v13, v14, v15, v16 etc estão disponíveis no momento em que este texto está sendo escrito.</p>
<p align='center'>Primeiro, instalaremos o PPA para obter acesso aos pacotes dele. Do seu diretório home, utilize o <strong>curl</strong> para recuperar o script de instalação para sua versão de preferência, certificando-se de substituir o <strong>16.x<strong> pela string da sua versão favorita (se for diferente)</p>
<p align='center'>Caso não tenha o <strong>curl</strong> use:</p>

```
sudo apt install curl
```
<p align='center'>Para instalar o node use os comandos abaixo:</p>
<br>
<p align='center'>Primeiro, instalaremos o PPA para obter acesso aos pacotes dele.</p>
```
cd ~
curl -sL https://deb.nodesource.com/setup_14.x -o nodesource_setup.sh
```
<p align='center'>execute o script com o <strong>sudo</strong>:</p>
```
sudo bash nodesource_setup.sh
```
<p align='center'>O PPA será adicionado à sua configuração e seu cache de pacotes local será atualizado automaticamente. Agora, você pode instalar o pacote Node.js</p>
```
sudo apt install nodejs
```
<p align='center'>Verifique se você instalou a nova versão executando o node com o sinalizador de versão -v:</p>
```
node -v
```