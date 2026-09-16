# Lab 01 – Azure Governance and Identity

## Objetivo

Aprender conceitos fundamentais de governança, identidade e controle de acesso no Microsoft Azure.

## Recursos estudados

- Azure Resource Groups
- Tags
- Cost Management
- Microsoft Entra ID
- Azure RBAC
- Least Privilege

## Cenário

Foi criado um ambiente de laboratório para estudos da certificação AZ-104.

### Resource Group criado

`rg-lab-az104-ananda`

### Tags configuradas

- Environment: LAB
- Project: AZ104
- Owner: Ananda
- CostCenter: Estudos

## Cost Management

Foi criado um orçamento para acompanhar os gastos do laboratório.

Nome do orçamento:

`budget-lab-az104`

Objetivo:

- acompanhar os custos do ambiente;
- evitar gastos inesperados;
- praticar conceitos de FinOps;
- compreender o uso de alertas de orçamento.

## Conceitos aprendidos

### Resource Group

Um Resource Group é uma forma de organizar recursos relacionados dentro do Azure.

### Tags

Tags são etiquetas usadas para organizar, identificar e classificar recursos.

Exemplos:

- ambiente;
- projeto;
- responsável;
- centro de custo.

### Cost Management

Cost Management é utilizado para acompanhar e analisar os custos dos recursos no Azure.

### Azure RBAC

RBAC significa Role-Based Access Control.

Ele permite controlar:

- quem pode acessar;
- o que a pessoa pode fazer;
- em quais recursos ela terá acesso.

## Prática realizada com Azure RBAC

Foi analisado o processo de atribuição de funções no Azure por meio de:

- Access control (IAM)
- Add role assignment
- Role: Reader
- Members
- User, group, or service principal
- Managed identity

### Conceitos observados

**Reader**  
Permite visualizar recursos, sem realizar alterações.

**Contributor**  
Permite criar e alterar recursos, mas não possui o mesmo nível de gerenciamento de acesso que o Owner.

**Owner**  
Permite administrar recursos e também controlar permissões.

### Herança de permissões

Foi observado que algumas permissões estavam marcadas como **Inherited**.

Isso significa que a permissão foi herdada de um nível superior, como:

Management Group → Subscription → Resource Group → Resource

### Least Privilege

Foi aplicado o conceito de menor privilégio:

um usuário deve receber somente as permissões necessárias para executar sua função.

### Tipos de identidade analisados

- User: pessoa
- Group: grupo de usuários
- Service principal: identidade usada por aplicações ou automações
- Managed identity: identidade gerenciada pelo próprio Azure para recursos

## Limitação encontrada

O acesso administrativo ao Microsoft Entra ID não estava disponível no tenant institucional utilizado no laboratório.

Por isso, a prática de criação de usuários e grupos no Entra ID ficou pendente.

Mesmo com essa limitação, foi possível praticar conceitos de RBAC e IAM diretamente no Resource Group.


## Status

✅ Resource Group criado  
✅ Tags configuradas  
✅ Budget configurado  
✅ Azure RBAC - fluxo de atribuição de funções analisado  
⏳ Microsoft Entra ID - acesso administrativo restrito no tenant institucional
