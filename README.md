# Descrição

Repositório com código para gerar o site da ONG Crescer

# Pré-requisitos

Ter um ambiente local com os seguintes serviços instalados e rodando:

- PHP >= 7.0
- MariaDB >= 10
- Apache >= 2.4
- NodeJS >= 6

Para usuários de windows recomendado o uso do [XAMPP](https://www.apachefriends.org/download.html).

# Instalação

Faça o clone do repositório direto no diretório em que o apache se encontra rodando.

```
git clone https://github.com/ongcrescer/wp-site.git
```

Acesse seu servidor local via navegador e prossiga com a instalação padrão do wordpress

Após a instalação do wordpress, selecione o tema da ONG a partir do menu `aparência -> temas`

# Desenvolvimento

Para ajudar a contribuir com a construção do site da ONG seguem alguns pontos importantes:

- O site da ONG é um tema em wordpress, recomendamos olhar o conteúdo de [criação de temas](https://www.wptotal.com/como-criar-um-wordpress-theme/)
- O css do site, é gerado usando [sass](http://sass-lang.com/guide) para facilitar o desenvolvimento

## Gostaria de contribui, por onde começo?

Tenha uma instalação do wordpress funcionadno com o tema da ONG ativado.

Abra seu terminal, linha de comando, e acesse o diretório do tema do wordpress:

```
# ex: wordpress instalado em C:\htdocs\wp-site\wp-content\themes\ongcrescer\

cd C:\htdocs\wp-site\wp-content\themes\ongcrescer\
```

Uma vez dentro do diretório instale as dependências do sass:

```
npm install -g yarn
yarn install
```

Será criado um diretório dentro do tema chamado, `node_modules` ele conterá o programa para trabalhar com
o css do tema.

Uma vez instalado rode o seguinte comando:

```
node_modules/brunch/bin/brunch watch
```

Este comando ficará olhando os arquivos dentro do diretório `themes/ongcrescer/scss`. Qualquer alteração nesses
arquivos será gerado um novo `style.css` na raiz do diretório do tema.


## Links úteis:

- [Como criar manter um theme no Wordpress](https://www.wptotal.com/como-criar-um-wordpress-theme/)
- [Como contribuir com o site](https://blog.da2k.com.br/2015/02/04/git-e-github-do-clone-ao-pull-request/)

## Canais de comunicação

Dúvidas de desenvolvimento entre em contato no nosso chat - [https://ongcrescer.slack.com/](Slack)
