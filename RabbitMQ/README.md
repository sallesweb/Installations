# RabbitMQ
Passo a passo da instalação do RabbitMQ em um servidor Windows.

## Instalação Erlang
O RabbitMQ depende da instalação do Erlang.  
> - [Download Erlang](https://www.erlang.org/downloads)

## Instalação RabbitMQ
Há várias formas de se instalar o servidor RabbitMQ, utilizaremos o *Windows Installer*.
> - [Download RabbitMQ Server](https://github.com/rabbitmq/rabbitmq-server/releases/download/v3.8.11/rabbitmq-server-3.8.11.exe)

### Confirmação de instalação
Execute o comando à seguir para confirmar se o RabbitMQ está instalado corretamente.
```cmd
    telnet 127.0.0.1 5672
```

## Habilitar interface RabbitMQ
Acesse a pasta de instalação do RabbitMQ e execute o comando para habilitar o plugin.
```cmd
    cd C:\Program Files\RabbitMQ Server\rabbitmq_server-3.8.11\sbin

    rabbitmq-plugins enable rabbitmq_management
```
### Confirmação de instalação
Execute o link à seguir para confirmar se o *Management* do RabbitMQ está funcionando corretamente.
> 127.0.0.1:15672

## Referências
- [Download Erlang](https://www.erlang.org/downloads)
- [Downloading and Installing RabbitMQ](https://www.rabbitmq.com/download.html)
- [Management Plugin](https://www.rabbitmq.com/management.html)