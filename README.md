# Droppy

## Descrição
Projeto baseado no repositório [DROPPY](https://github.com/silverwind/droppy.git). Ele tem a capacidade de criar um servidor parecido com um dropbox.

Foi criado para ser uma forma mais built in para criar seus servidores. 

## Dependências
* Docker 
~~~bash
sudo apt install docker.io
sudo usermod -aG docker $USER
~~~

* docker-compose 
~~~bash
# Baixa o docker-compose no seu desktop linux
sudo curl -L "https://github.com/docker/compose/releases/download/1.26.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

# O transforma em executável
sudo chmod +x /usr/local/bin/docker-compose

# Cria um link para o /usr/bin para ir para o PATH
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
~~~

## Executar
~~~bash
git clone https://github.com/viniciusecortez/droppy-built-in.git ~/app
cd ~/app
docker-compose build
docker-compose up
~~~