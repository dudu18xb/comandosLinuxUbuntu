## comandos linux para instalar arquivos todos os codigos foram testados no Ubuntu 17.10


### Instalar o pacote completo do LAMP que vem o Apache, Mysql, PHP 7.1 
> sudo apt-get install lamp-server^


### Instalando o phpmyadmin
> sudo apt-get install phpmyadmin 


### Instalando o sublime 3 pelo terminal
> sudo wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -

> sudo apt-get install apt-transport-https

> sudo echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list

> sudo apt-get update

> sudo apt-get install sublime-text


### Instalando o Composer 
> sudo apt-get install curl

> curl -sS https://getcomposer.org/installer | php

> chmod +x composer.phar

> mv composer.phar /usr/local/bin/composer

> composer self-update

### Instalando o phpstorn

- Abaixa o Arquivo no site

- https://www.jetbrains.com/phpstorm/download/#section=linux

- Renomeia o arquivo abaixado para phpstorm.tar.gz

- Use o comando a seguir para descompactar o arquivo baixado

> sudo tar vzxf phpstorm.tar.gz -C /opt/

 - Renomeie a pasta criada. Se ao executar o comando abaixo ocorrer um erro com a mensagem iniciando com “mv: é impossível sobrescrever o não-diretório”, pule este passo

> sudo mv /opt/PhpStorm*/ /opt/phpstorm

- Finalmente, crie um atalho para facilitar a execução do programa

> sudo ln -sf /opt/phpstorm/bin/phpstorm.sh /usr/bin/phpstorm

- Se seu ambiente gráfico atual suportar, crie um lançador para o programa, executando o comando abaixo;

> echo -e '[Desktop Entry]\n Version=1.0\n Name=phpstorm\n Exec=/opt/phpstorm/bin/phpstorm.sh\n Icon=/opt/phpstorm/bin/phpstorm.png\n Type=Application\n Categories=Application' | sudo tee /usr/share/applications/phpstorm.desktop

