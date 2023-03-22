Download de dados da Internet
Faça o download e normalize os dados da Internet de várias fontes. Este pacote é normalmente executado diariamente (após as 10:00 CST).

Dependências
Ubuntu

sudo apt-get install coreutils build-essential libssl-dev curl gnupg pigz liblz4-tool

Ruby

Ubuntu 16.04 LTS

sudo apt-get install ruby

Outras distribuições

gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
\curl -sSL https://get.rvm.io | bash -s stable --ruby=2.3.3


O processo de normalização depende das ferramentas fornecidas pelo projeto inetdata-parsers. Por favor, consulte o README para obter mais informações. As ferramentas inetdata-parsers precisam estar no caminho do sistema para que o processo de normalização seja concluído.

Limites do sistema
O processo de normalização requer um grande número de identificadores de arquivo abertos. Se o normalizador for executado como root, ele tentará modificar o r
