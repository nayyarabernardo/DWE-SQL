# Projeto ETL com SCD2

Este projeto realiza uma ETL utilizando o método SCD2 (Slowly Changing Dimension 2) para a transformação de dados brutos do banco de dados Northwind. A modelagem é composta por quatro esquemas: STAGING, SILVER, GOLD e LOGS. O processo inclui a criação de uma tabela de log e uma procedure de log para reutilização nos diversos processos. Uma tabela STAGING é desenvolvida para receber os dados brutos, permitindo uma carga bulk otimizada.

### Carga Bulk Otimizada

O processo de carga é otimizado com a utilização de bulk load, proporcionando eficiência na transferência dos dados para as tabelas. O esquema GOLD armazena as informações consolidadas para análises.

### Procedimento de Log Reutilizável

Um procedimento de log foi criado para registrar informações sobre o processo de carga, possibilitando monitoramento e análise de eventos. A procedure é flexível e pode ser reutilizada em diferentes processos ETL.

## Pré-requisitos

    Banco de dados Microsoft SQL Server
    Azure Data Studios

## Como usar

    Clone o repositório para sua máquina local
    Abra o Azure Data Studios e carregue o arquivo .ipynb desejado
    Conecte-se ao seu banco de dados Microsoft SQL Server
    Execute as células de código no notebook

Obs: As células de código devem ser executadas na ordem em que aparecem no arquivo para garantir o correto funcionamento da ETL.

## Contribuições

Contribuições são sempre bem-vindas e apreciadas. Para fazer uma contribuição, por favor, abra uma solicitação de pull.
