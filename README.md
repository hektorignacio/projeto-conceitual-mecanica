# projeto-conceitual-mecanica

# Sistema de Gestão para Oficina Mecânica

## Descrição
Este projeto tem como objetivo fornecer um sistema de gestão para oficinas mecânicas, facilitando o controle de clientes, veículos, ordens de serviço, estoque e fornecedores. O modelo de dados foi estruturado para permitir um fluxo de trabalho eficiente e organizado.

## Modelo de Dados
O sistema é baseado em um banco de dados relacional com as seguintes entidades:

### 1. Clientes
Armazena informações sobre os clientes da oficina.
- Nome
- CPF
- CNPJ
- ID
- Endereço
- Telefone
- Email
- Veículo (relacionado à tabela **Veículos**)

### 2. Veículos
Registra os veículos dos clientes.
- ID
- Modelo
- Marca
- Cor
- Ano
- Placa
- Tipo

### 3. Empregados
Guarda informações sobre os funcionários da oficina.
- Nome
- CPF
- ID
- Profissão
- Endereço
- Telefone
- Email

### 4. Ordem de Serviço
Gerencia as ordens de serviço da oficina.
- ID
- Status
- Data de Início
- Data de Conclusão
- Preço
- Data de Pagamento
- ID Veículo (relacionado à tabela **Veículos**)
- ID Cliente (relacionado à tabela **Clientes**)
- ID Empregado (relacionado à tabela **Empregados**)

### 5. Fornecedores
Contém informações sobre os fornecedores da oficina.
- ID
- CNPJ
- Endereço
- Telefone
- Email

### 6. Estoque
Gerencia as peças disponíveis para manutenção.
- ID Peças
- Preço de Revenda
- Preço de Compra
- Quantidade

### 7. Serviços Oferecidos
Lista os serviços disponíveis na oficina.
- ID
- Tipo de Serviço
- Preço
- Duração
- Descrição
