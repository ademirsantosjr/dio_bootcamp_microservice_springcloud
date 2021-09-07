# Aplicação de exemplo, com arquitetura baseada em microserviços usando Spring Cloud

Aplicação construída com base no _live-coding_ do _bootcamp_ 'Santander Full-Stack Developer' na plataforma da Digital Innovation One, demonstrando uma arquitetura composta por dois seriços: 'product-catalog' e 'shopping-cart', que utilizam, respectivamente, a _search engine_ Elasticsearch e a estrutura de armazenamento Redis. Nesta aplicação foram definidas as classes _Config Server_, _Service Discovery_ e _Gateway_  

## Requisitos

* Java 11
* Gradle 7.2
* Elasticsearch 7.12.1
* Redis (versão mais recente)

## _Build_ da aplicação

* Construir cada aplicação utilizando o seguinte comando:

```bash
./gradlew build -x test
```

* Executar cada aplicação utilizando o seguinte comando:

```bash
./gradlew bootRun
```

## Executar a aplicação

* Passos a seguir:

1. Manter o Elasticsearch e o Redis em execução
2. Executar a aplicação de Configuração do Servidor disponível na pasta "configserver" ou no _link_ a seguir:
   1. https://github.com/ademirsantosjr/dio_bootcamp_microservice_springcloud_configserver
3. Executar a aplicação para Descoberta dos Serviços disponíveis na pasta "servicediscover" ou no _link_ a seguir:
   1. https://github.com/ademirsantosjr/dio_bootcamp_microservice_springcloud_servicediscovery
4. Executar a aplicação de _Gateway_ disponível na pasta "gateway" ou no _link_ a seguir:
   1. https://github.com/ademirsantosjr/dio_bootcamp_microservice_springcloud_gateway
5. Expor o serviço 'product-catalog' executando a aplicação disponível na pasta "productcatalog" ou no _link_ a seguir:
   1. https://github.com/ademirsantosjr/dio_bootcamp_microservice_springcloud_elasticsearch
6. Expor o serviço 'shopping-cart' executando a aplicação da pasta "shoppingcart" ou do _link_ a seguir
   1. https://github.com/ademirsantosjr/dio_bootcamp_microservice_springcloud_redis

> Nota: as configurações da aplicação apontam para os arquivos .yml deste repositório Git.
