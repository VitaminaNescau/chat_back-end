
# Chat Server

Este é um servidor back-end para um chat utilizando `ServerSocket` Java e a API JAX-RS com Reactor Netty.

# Pré-requisitos

Certifique-se de ter as seguintes ferramentas instaladas:

- JDK (Java Development Kit)
- Maven

# Configuração

1. Clone este repositório para o seu ambiente local:
  
  git clone https://github.com/vitaminanescau/chat_back-end.git

2. Acesse o diretório do projeto:


3. Compile o projeto usando o Maven:

  mvn clean package

# Executando o servidor

Após a configuração, você pode iniciar o servidor executando o seguinte comando:

java -jar Servidor.jar

O servidor estará em execução e pronto para receber conexões de clientes para o chat na porta 3030 da rede local.

# Uso do ServerSocket

O servidor utiliza o ServerSocket para lidar com as conexões de clientes. O ServerSocket é responsável por ouvir e aceitar conexões de entrada dos clientes na porta 3030.

O código para o uso do ServerSocket pode ser encontrado no arquivo `ServerDK.java`. Ele estabelece uma conexão com cada cliente e gerencia as mensagens recebidas e enviadas.

# Uso da API

Este servidor oferece uma API baseada em JAX-RS para gerenciar as operações do chat. Abaixo estão alguns exemplos de endpoints disponíveis:

- `GET /friends/list/{id}`: Obtém a lista de amigos do usuário.
- `GET /friends/list/new/{user_name}/{name}`: Adiciona um amigos ao usuário.
- `GET /messager/{id}/{name}`: Obtém o histórico de mensagens.
- `POST /singup`: Cria um novo usuario.

Os endpoints `/friends`, `/messager` e `/singup` são apenas exemplos, e você pode ajustá-los de acordo com as necessidades do seu projeto.

Consulte a documentação da API para obter detalhes completos sobre os endpoints disponíveis e como usá-los.
