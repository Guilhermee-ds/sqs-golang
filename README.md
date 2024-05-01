# Projeto SQS com Golang e AWS para Envio e Leitura de Mensagens

### Descrição do Projeto

Este projeto implementa um sistema de fila para envio e leitura de mensagens utilizando o Amazon SQS e a linguagem de programação Golang. O objetivo principal é demonstrar como criar, consumir e gerenciar filas no SQS com Golang, permitindo a comunicação assíncrona entre diferentes aplicações ou serviços.

## Funcionalidades

- Criação e gerenciamento de filas SQS
- Envio de mensagens para filas SQS
- Leitura e processamento de mensagens de filas SQS
- Tratamento de erros e exceções
- Monitoramento de filas SQS

## Tecnologias Utilizadas:

- Golang
- Amazon SQS
- AWS SDK for Golang
- AWS CLI

## Dependências:

- Golang >= go1.22.1
- AWS CLI

## Como Rodar

Depois de ter todas a dependências informadas anteriormente

Faça o Build do seu projeto

```shell
go build main.go
```

Crie uma fila na AWS

```shell
aws --profile seu-perfil-na-aws sqs create-queue --queue-name my-queue
```

Inicie o programa

```shell
go run main.go
```

Envie a mensagen para a fila

```shell
aws --profile seu-perfil-na-aws sqs send-message --queue-url http://sqs.us-east-1.localhost.localstack.cloud:4566/000000000000/my-queue --message-body "olá, essa é a minha mensagem com golang na aws"

```

Volte para o terminal aonde está com o arquivo main sendo rodado e lá estará a sua mensagem enviada 🎉

## Autores

- [@Guilherme Oliveira](https://www.linkedin.com/in/guilhermee-oliveiraa/)
