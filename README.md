# Esquema-Conceitual-oficina
Construindo um Esquema Conceitual para Banco De dados DIO Bootcamp Database Experience

Etapas do Desenvolvimento
Identificar Entidades: Clientes, Veículos, Mecânicos, Equipes, Ordem de Serviço (OS), Serviços, e Peças.
Definir Atributos: Associar a cada entidade os atributos relevantes descritos na narrativa.
Estabelecer Relacionamentos: Relacionar as entidades para modelar o processo do sistema.
Esquema Conceitual (Descrição)
Entidades e Atributos
Cliente

Código do cliente (PK)
Nome
Endereço
Telefone
Veículo

Placa (PK)
Modelo
Marca
Ano
Código do cliente (FK)
Mecânico

Código do mecânico (PK)
Nome
Endereço
Especialidade
Equipe

Código da equipe (PK)
Nome da equipe
Ordem de Serviço (OS)

Número da OS (PK)
Data de emissão
Data de conclusão prevista
Valor total
Status
Código do cliente (FK)
Código da equipe (FK)
Serviço

Código do serviço (PK)
Descrição
Valor de mão de obra
Peça

Código da peça (PK)
Descrição
Valor unitário
Relacionamentos
Cliente tem um ou mais Veículos

1:N (Um cliente pode ter vários veículos, mas cada veículo pertence a um cliente).
Veículo gera uma Ordem de Serviço (OS)

1:N (Um veículo pode ter várias ordens de serviço).
Equipe é responsável por uma ou mais OS

1:N (Uma equipe pode ser designada para várias ordens de serviço).
Equipe é composta por Mecânicos

N:M (Uma equipe pode ter vários mecânicos e cada mecânico pode fazer parte de várias equipes).
OS inclui Serviços

N:M (Uma ordem de serviço pode incluir vários serviços, e um serviço pode estar em várias OS).
OS utiliza Peças

N:M (Uma ordem de serviço pode utilizar várias peças, e uma peça pode ser utilizada em várias OS).

![Diagrama_Oficina](https://github.com/user-attachments/assets/159087b6-0e1b-4b19-b57c-ab85a5cd9f3b)


