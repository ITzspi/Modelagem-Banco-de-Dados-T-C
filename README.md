# Loja Traias e Catiras

# Cenário
Uma selaria chamada "Traias e Catiras" deseja implementar um sistema de gerenciamento para armazenar informações sobre seus clientes e vendedores. A empresa pretende melhorar o atendimento ao cliente e manter um registro organizado das transações, o que inclui informações sobre os compradores e os vendedores envolvidos. 

# Entidades e Atributos 
  Entidade: Cliente 
Atributos: 
ID do Cliente,
Nome, 
Endereço (composto: Rua, Cidade, CEP), 
Telefone, 
Multivalorado: Compras Anteriores.  

Entidade: Vendedor 
Atributos: 
ID do Vendedor,  
Nome, 
Telefone, 
Comissão.  

Entidade: Produto 
Atributos:
ID do Produto,  
Nome, 
Descrição, 
Preço, 
Estoque Disponível, 
Multivalorado: Fornecedor (nome do fornecedor e informações de contato). 

Entidade: Compra 
Atributos: 
ID da Compra,  
Dados da Compra, 
Valor total, 
Forma de Pagamento, 
Chave Estrangeira: ID do Cliente,  
Chave Estrangeira: ID do Vendedor (para associar a compra a um vendedor). 

# Relacionamentos
 Relacionamento 1:N entre Cliente e Compra: 
Um cliente pode realizar várias compras, mas uma compra pertence a apenas um cliente. 

Relacionamento 1:N entre Vendedor e Cliente: 
Um vendedor pode estar envolvido em várias compras de clientes, e clientes pode ter comprado com outros vendedores 

Relacionamento N:N entre Produto e Compra:
Muitos produtos podem ser comprados em muitas compras, representando quais produtos foram comprados em cada transação. 

Relacionamento 1:N entre Produto e Fornecedor: 
Um produto pode ser fornecido por vários fornecedores 
    
# Diagrama Entidade-Relacionamento
![der](https://github.com/pblcnr/Trabalho_LojaMaisVinil/assets/141787223/f914f785-b66c-4bff-88cd-77f43fbaa107)

# Modelagem Lógica
![modelo lógico](https://github.com/pblcnr/Trabalho_LojaMaisVinil/assets/141787223/678c9cd6-86ef-40d4-8c5f-8882b5146d98)

# Dados
  Todos os scripts de Dados estão no arquivo 'Loja MaisVinil.sql'
  
# CRUD
  Todos os Scripts de CRUD estão na pasta 'CRUD'

# Relatórios 
  Todos os Scripts de Relatórios estão na pasta 'Relatórios'
