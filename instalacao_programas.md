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

> $ sudo rm -Rf /opt/phpstorm*


> $ sudo rm -Rf /usr/bin/phpstorm


> $ sudo rm -Rf /usr/share/applications/phpstorm.desktop


Pronto agora podemos baixar-lo e instala-lo com os seguintes comandos:
> $ wget https://download.jetbrains.com/webide/PhpStorm-2017.3.tar.gz \ -O phpstorm.tar.gz

Descompactando em pasta /opt/:
> $ sudo tar vzxf phpstorm.tar.gz


Alterando o nome da pasta:
> $ sudo mv /opt/PHPStorm*/  /opt/phpstorm



Criando Link simbólico para pasta /usr/bin:


> $ sudo ln -sf /opt/phpstorm/bin/phpstorm.sh /usr/bin/phpstorm


Criar lançador para o programa:

> $ echo -e '[Desktop Entry]\n Version=1.0\n Name=phpstorm\n \ 
Exec=/opt/phpstorm/bin/phpstorm.sh\n Icon=/opt/phpstorm/bin/phpstorm.png\n \
 Type=Application\n Categories=Application' \ 
| sudo tee /usr/share/applications/phpstorm.desktop


Concedendo permissão para executar o lançador:
> $ sudo chmod +x /usr/share/applications/phpstorm.desktop

Entrando no arquivos de Hosts no Ubuntu:
> $ sudo nano /etc/hosts