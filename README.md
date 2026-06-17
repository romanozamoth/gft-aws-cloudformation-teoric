# Desafio DIO - Infraestrutura Automatizada com AWS CloudFormation

## Descrição

Este repositório foi desenvolvido como parte do laboratório da DIO com foco na automação de infraestrutura utilizando AWS CloudFormation.

O objetivo foi compreender como provisionar ambientes completos através de Infrastructure as Code (IaC), eliminando configurações manuais e aumentando a padronização dos recursos na nuvem.

---

# Objetivos do Laboratório

* Aplicar conceitos de Infrastructure as Code.
* Automatizar a criação de recursos AWS.
* Utilizar Templates CloudFormation.
* Provisionar infraestrutura de forma padronizada.
* Documentar os conhecimentos adquiridos.

---

# Visão Geral da Solução

A infraestrutura foi definida utilizando AWS CloudFormation, permitindo a criação automatizada de recursos através de templates declarativos.

Fluxo utilizado:

Template → CloudFormation → Stack → Recursos AWS

---

# Conceitos Utilizados

## Infrastructure as Code (IaC)

Modelo de gerenciamento onde a infraestrutura é descrita em arquivos versionáveis.

Benefícios:

* Automação
* Padronização
* Reprodutibilidade
* Controle de mudanças
* Escalabilidade

---

## AWS CloudFormation

Serviço responsável por criar e gerenciar recursos AWS a partir de templates YAML ou JSON.

---

## Stack

Conjunto de recursos criados e gerenciados pelo CloudFormation.

Uma Stack pode conter diversos recursos relacionados:

* EC2
* VPC
* Security Groups
* S3
* IAM
* Load Balancer

---

# Recursos Provisionados

Durante o laboratório foram criados recursos automatizados utilizando CloudFormation.

Exemplos:

* Instâncias EC2
* Grupos de Segurança
* Recursos de Rede
* Serviços de Armazenamento

---

# Etapas Executadas

## 1. Criação do Template

Definição da infraestrutura em arquivos YAML.

---

## 2. Validação

Verificação da sintaxe e integridade do template.

---

## 3. Criação da Stack

Envio do template para o CloudFormation realizar o provisionamento automático.

---

## 4. Monitoramento

Acompanhamento dos eventos da Stack:

* CREATE_IN_PROGRESS
* CREATE_COMPLETE
* UPDATE_IN_PROGRESS
* UPDATE_COMPLETE
* DELETE_COMPLETE

---

## 5. Validação dos Recursos

Confirmação da criação correta dos recursos provisionados.

---

# Estrutura de Template

Exemplo simplificado:

```yaml
AWSTemplateFormatVersion: '2010-09-09'

Resources:
  WebServer:
    Type: AWS::EC2::Instance
    Properties:
      InstanceType: t2.micro
```

---

# Benefícios Observados

* Redução de configurações manuais
* Rapidez na criação de ambientes
* Padronização da infraestrutura
* Facilidade de replicação
* Melhor governança dos recursos

---

# Insights Pessoais

O laboratório demonstrou na prática como Infrastructure as Code simplifica a administração de ambientes em nuvem.

A utilização do CloudFormation permite criar ambientes reproduzíveis, reduzindo erros operacionais e facilitando a manutenção da infraestrutura ao longo do tempo.

Também foi possível perceber a importância do versionamento dos templates para ambientes corporativos e processos DevOps.

---

# Conclusão

A prática permitiu compreender o funcionamento do AWS CloudFormation como ferramenta de automação de infraestrutura, reforçando conceitos de Infrastructure as Code, provisionamento automatizado e gerenciamento centralizado de recursos na AWS.
