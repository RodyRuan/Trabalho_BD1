# TRABALHO 01:  Título do Trabalho
Trabalho desenvolvido durante a disciplina de BD1

# Sumário

### 1. COMPONENTES<br>
Integrantes do grupo<br>
RUAN RODY DE MELO DA COSTA - RUAN-RODY@HOTMAIL.COM
GABRIEL MOROSINI - email_segundo_componente@dominio.com<br>
LUCAS DIAS ROCHA - email_segundo_componente@dominio.com<br>
MIGUEL MALINII - email_segundo_componente@dominio.com<br>


### 2.INTRODUÇÃO E MOTIVAÇÃO<br>
Este documento contém a especificação do projeto do banco de dados do FitMarket, um marketplace de academia e suplementação online. A motivação para o desenvolvimento desse sistema surge da necessidade de conectar fornecedores de produtos de academia e suplementação aos consumidores que buscam esses produtos. O FitMarket visa proporcionar praticidade e variedade aos consumidores, assim como aumentar a visibilidade e alcance dos produtos dos fornecedores no mercado. Para garantir o funcionamento adequado do sistema, é necessário que os fornecedores cadastrem seus produtos e os consumidores possam navegar pelo catálogo, selecionar e comprar os produtos desejados
 

### 3.MINI-MUNDO<br>

> O FitMarket é um marketplace de academia e suplementação, é um sistema online que tem como objetivo conectar fornecedores de produtos de academia e suplementação aos consumidores que buscam esses produtos. O sistema permitirá que os fornecedores cadastrem seus produtos e os consumidores possam navegar pelo catálogo, selecionar e comprar produtos. Para que o sistema funcione corretamente, os fornecedores precisam se cadastrar na plataforma e fornecer informações sobre seus produtos, como nome, descrição, preço e imagens. Os consumidores, por sua vez, podem criar uma conta na plataforma para acessar o catálogo completo e fazer compras. Ao navegar pelo catálogo, os consumidores podem filtrar os produtos por categoria, marca, preço e outras características. Eles também podem ver avaliações e comentários de outros compradores sobre os produtos. Quando um consumidor decide fazer uma compra, ele pode adicionar os produtos ao carrinho e finalizar a compra com um sistema de pagamento seguro e confiável. Depois que a compra é confirmada, os fornecedores são notificados e enviam os produtos para a entrega. Um produto pode ser associado a vários vendedores. O FitMarket pode ser uma ótima opção para consumidores que buscam praticidade e variedade na hora de adquirir produtos de academia e suplementação, assim como para fornecedores que desejam aumentar a visibilidade e alcance de seus produtos no mercado

### 4.PROTOTIPAÇÃO, PERGUNTAS A SEREM RESPONDIDAS E TABELA DE DADOS<br>
#### 4.1 RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
Neste ponto a codificação não e necessária, somente as ideias de telas devem ser criadas, o princípio aqui é pensar na criação da interface para identificar possíveis informações a serem armazenadas ou descartadas <br>

Sugestão: https://balsamiq.com/products/mockups/<br>

![Alt text](https://github.com/discipbd1/trab01/blob/master/balsamiq.png?raw=true "Title")
![Arquivo PDF do Protótipo Balsamiq feito para Empresa Devcom](https://github.com/discipbd1/trab01/blob/master/arquivos/EmpresaDevcom.pdf?raw=true "Empresa Devcom")
#### 4.2 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?

> A Empresa FitMarket precisa inicialmente dos seguintes relatórios:
1- Relatório de vendas por fornecedor: Apresenta o total de vendas realizadas por cada fornecedor cadastrado no sistema, permitindo avaliar o desempenho de cada parceiro.

2- Relatório de estoque baixo: Lista os produtos que estão com quantidade abaixo de um limite pré-definido, auxiliando na identificação de produtos que precisam ser repostos.

3- Relatório de produtos mais vendidos: Apresenta os produtos que tiveram maior volume de vendas em um determinado período, permitindo identificar os itens mais populares entre os consumidores.

4- Relatório de avaliações e comentários por produto: Exibe as avaliações e comentários dos consumidores sobre cada produto, fornecendo insights sobre a qualidade e aceitação dos produtos.

5- Relatório de análise de mercado: Apresenta informações sobre as tendências do mercado de academia e suplementação, como demanda por categorias de produtos, marcas mais populares e variações de preços, auxiliando na identificação de oportunidades e no planejamento estratégico.

 
 
#### 4.3 TABELA DE DADOS DO SISTEMA:
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados 
    
![Exemplo de Tabela de dados da Empresa Devcom](https://github.com/discipbd1/trab01/blob/master/arquivos/TabelaEmpresaDevCom_sample.xlsx?raw=true "Tabela - Empresa Devcom")
    
    
### 5.MODELO CONCEITUAL

    ![image](https://github.com/RodyRuan/Trabalho_BD1/assets/112021384/d691f0a8-2d04-472b-ba14-fb52ddd25d40)
    
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Nomes dos que participaram na avaliação]
    [Grupo02]: [Nomes dos que participaram na avaliação]

#### 5.2 Descrição dos dados 
 Tabela FORNECEDOR:

Campo ID: Armazena o identificador único de cada fornecedor cadastrado no sistema. Esse campo é usado como chave primária para identificar os registros na tabela.
Campo NOME: Armazena as informações do nome do fornecedor.
Campo TELEFONE: Armazena o número de telefone do fornecedor.
Campo SENHA: Armazena a senha de acesso do fornecedor ao sistema.
Campo EMAIL: Armazena o endereço de email do fornecedor.

Tabela PRODUTOS_CATEGORIA:

Campo ID: Armazena o identificador único de cada produto cadastrado no sistema. Esse campo é usado como chave primária para identificar os registros na tabela.
Campo DESCRICAO: Armazena a descrição do produto.
Campo VALOR: Armazena o valor do produto.
Campo CATEGORIA: Armazena a categoria do produto.
Tabela CLIENTE:

Campo ID: Armazena o identificador único de cada cliente cadastrado no sistema. Esse campo é usado como chave primária para identificar os registros na tabela.
Campo NOME: Armazena as informações do nome do cliente.
Campo TELEFONE: Armazena o número de telefone do cliente.
Campo EMAIL: Armazena o endereço de email do cliente.
Campo SENHA: Armazena a senha de acesso do cliente ao sistema.
Campo ENDERECO: Armazena o endereço do cliente.

Tabela COMPRA:

Campo ID: Armazena o identificador único de cada compra realizada no sistema. Esse campo é usado como chave primária para identificar os registros na tabela.
Campo DATA: Armazena a data da compra.
Campo ID_PRODUTO: Armazena o identificador do produto comprado.
Campo ID_CLIENTE: Armazena o identificador do cliente que realizou a compra.
Campo ID_VENDEDOR: Armazena o identificador do fornecedor responsável pela venda.
Campo NOTA: Armazena a nota ou avaliação dada pelo cliente à compra.

Tabela ITEM_COMPRA:

Campo FK_COMPRA_ID: Armazena o identificador da compra à qual o item pertence, estabelecendo uma relação com a tabela COMPRA.
Campo FK_PRODUTOS_ID: Armazena o identificador do produto comprado, estabelecendo uma relação com a tabela PRODUTOS_CATEGORIA.
Campo QTD: Armazena a quantidade do produto comprada.

Tabela ADICIONA_NO_CARRINHO:

Campo FK_CLIENTE_ID: Armazena o identificador do cliente que adicionou o produto ao carrinho, estabelecendo uma relação com a tabela CLIENTE.
Campo FK_PRODUTOS_CATEGORIA_ID: Armazena o identificador do produto adicionado ao carrinho, estabelecendo uma relação com a tabela PRODUTOS_CATEGORIA.
Campo ID_PRODUTO: Armazena o identificador do produto adicionado ao carrinho.
Campo QTD: Armazena a quantidade do produto adicionada ao carrinho, indicando a quantidade de itens que o cliente deseja comprar.

Tabela VENDE:

Campo FK_FORNECEDOR_ID: Armazena o identificador do fornecedor responsável pela venda, estabelecendo uma relação com a tabela FORNECEDOR.
Campo FK_PRODUTOS_CATEGORIA_ID: Armazena o identificador do produto vendido, estabelecendo uma relação com a tabela PRODUTOS_CATEGORIA.
Campo ID_PRODUTO: Armazena o identificador do produto vendido.
Campo QTD: Armazena a quantidade do produto vendida pelo fornecedor.


### 6	MODELO LÓGICO<br>

        ![image](https://github.com/RodyRuan/Trabalho_BD1/assets/112021384/6e049856-c012-4cb5-9990-c36f29cf462f)

### 7	MODELO FÍSICO

CREATE TABLE fornecedor (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(60),
    telefone VARCHAR(60),
    senha VARCHAR(60),
    email VARCHAR(60)
);

CREATE TABLE produtos_categoria (
    id SERIAL PRIMARY KEY,
    descricao VARCHAR(60),
    valor FLOAT,
    categoria VARCHAR(60)
);

CREATE TABLE cliente (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(60),
    telefone VARCHAR(60),
    email VARCHAR(60),
    senha VARCHAR(60),
    endereco VARCHAR(60)
);

CREATE TABLE compra (
    id SERIAL PRIMARY KEY,
    data DATE,
    id_produto INT,
    id_cliente INT,
    id_vendedor INT,
    nota FLOAT,
    FOREIGN KEY (id_produto) REFERENCES produtos_categoria(id),
    FOREIGN KEY (id_cliente) REFERENCES cliente(id),
    FOREIGN KEY (id_vendedor) REFERENCES fornecedor(id)
);

CREATE TABLE vende (
    fk_fornecedor_id INT,
    fk_produtos_id INT,
    FOREIGN KEY (fk_fornecedor_id) REFERENCES fornecedor(id),
    FOREIGN KEY (fk_produtos_id) REFERENCES produtos_categoria(id),
    PRIMARY KEY (fk_fornecedor_id, fk_produtos_id)
);

CREATE TABLE item_compra (
    fk_compra_id INT,
    fk_produtos_id INT,
    qtd INT,
    FOREIGN KEY (fk_compra_id) REFERENCES compra(id),
    FOREIGN KEY (fk_produtos_id) REFERENCES produtos_categoria(id),
    PRIMARY KEY (fk_compra_id, fk_produtos_id)
);

CREATE TABLE adiciona_no_carrinho (
    fk_cliente_id INT,
    fk_produtos_categoria_id INT,
    id_produto INT,
    qtd INT,
    FOREIGN KEY (fk_cliente_id) REFERENCES cliente(id),
    FOREIGN KEY (fk_produtos_categoria_id) REFERENCES produtos_categoria(id),
    PRIMARY KEY (fk_cliente_id, fk_produtos_categoria_id)
);
 
        
       
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
   -- Inserções na tabela fornecedor
   INSERT INTO fornecedor (nome, telefone, senha, email)
   VALUES
       ('João Silva', '+55 11 91234-5678', 'senha123', 'joao.silva@example.com'),
       ('Maria Santos', '+55 21 98765-4321', 'senha456', 'maria.santos@example.com'),
       ('Pedro Almeida', '+55 31 99876-5432', 'senha789', 'pedro.almeida@example.com'),
       ('Ana Costa', '+55 41 98765-4321', 'senha012', 'ana.costa@example.com'),
       ('Lucas Oliveira', '+55 51 91234-5678', 'senha345', 'lucas.oliveira@example.com');

   -- Inserções na tabela produtos_categoria
   INSERT INTO produtos_categoria (descricao, valor, categoria)
   VALUES
       ('Camiseta Esportiva', 29.99, 'Vestuário'),
       ('Whey Protein', 59.99, 'Suplementos'),
       ('Tênis de Corrida', 129.99, 'Calçados'),
       ('Barras de Proteína', 19.99, 'Suplementos'),
       ('Shorts de Academia', 39.99, 'Vestuário'),
       ('Creatina', 24.99, 'Suplementos'),
       ('Legging Fitness', 49.99, 'Vestuário'),
       ('Luvas para Musculação', 14.99, 'Acessórios'),
       ('Pré-Treino', 34.99, 'Suplementos'),
       ('Corda de Pular', 9.99, 'Acessórios');

   -- Inserções na tabela cliente
   INSERT INTO cliente (nome, telefone, email, senha, endereco)
   VALUES
       ('Fernanda Lima', '+55 11 92345-6789', 'fernanda.lima@example.com', 'senha123', 'Rua das Flores, 123'),
       ('Ricardo Martins', '+55 21 99876-5432', 'ricardo.martins@example.com', 'senha456', 'Avenida Principal, 456'),
       ('Carolina Ferreira', '+55 31 98765-4321', 'carolina.ferreira@example.com', 'senha789', 'Travessa das Ruas, 789'),
       ('Marcos Oliveira', '+55 41 91234-5678', 'marcos.oliveira@example.com', 'senha012', 'Praça Central, 012'),
       ('Juliana Silva', '+55 51 99876-5432', 'juliana.silva@example.com', 'senha345', 'Alameda dos Bosques, 345');

   -- Inserções na tabela compra
   INSERT INTO compra (data, id_produto, id_cliente, id_vendedor, nota)
   VALUES
       ('2023-05-05', 1, 1, 1, 4.5),
       ('2023-05-06', 2, 1, 2, 5),
       ('2023-05-07', 3, 2, 3, 4),
       ('2023-05-08', 4, 2, 1, 3.5),
       ('2023-05-09', 5, 3, 3, 4),
       ('2023-05-10', 6, 3, 2, 5),
       ('2023-05-11', 7, 4, 4, 4.5),
       ('2023-05-12', 8, 4, 3, 4.5),
       ('2023-05-13', 9, 5, 2, 4),
       ('2023-05-14', 10, 5, 1, 4.5);

   -- Inserções na tabela vende
   INSERT INTO vende (fk_fornecedor_id, fk_produtos_id)
   VALUES
       (1, 1),
       (2, 2),
       (2, 3),
       (3, 4),
       (3, 5),
       (4, 6),
       (4, 7),
       (5, 8),
       (5, 9),
       (1, 10);

   -- Inserções na tabela item_compra
   INSERT INTO item_compra (fk_compra_id, fk_produtos_id, qtd)
   VALUES
       (1, 1, 2),
       (1, 2, 1),
       (2, 2, 3),
       (2, 3, 2),
       (3, 4, 1),
       (3, 5, 1),
       (4, 6, 2),
       (4, 7, 3),
       (5, 8, 1),
       (5, 9, 3);

   -- Inserções na tabela adiciona_no_carrinho
   INSERT INTO adiciona_no_carrinho (fk_cliente_id, fk_produtos_categoria_id, id_produto, qtd)
   VALUES
       (1, 1, 1, 1),
       (1, 2, 2, 2),
       (2, 2, 3, 1),
       (2, 3, 4, 3),
       (3, 4, 5, 1),
       (3, 5, 6, 2),
       (4, 6, 7, 1),
       (4, 7, 8, 3),
       (5, 8, 9, 1),
       (5, 9, 10, 2);



### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

># Marco de Entrega 01: Do item 1 até o item 9.1<br>

#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>
#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas

#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.

#### 9.5	INSTRUÇÕES APLICANDO ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>
    a) Criar minimo 3 de exclusão
    b) Criar minimo 3 de atualização

#### 9.6	CONSULTAS COM INNER JOIN E ORDER BY (Mínimo 6)<br>
    a) Uma junção que envolva todas as tabelas possuindo no mínimo 2 registros no resultado
    b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>
    a) Criar minimo 2 envolvendo algum tipo de junção

#### 9.8	CONSULTAS COM LEFT, RIGHT E FULL JOIN (Mínimo 4)<br>
    a) Criar minimo 1 de cada tipo

#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join (caso não ocorra na base justificar e substituir por uma view)
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho

#### 9.10	SUBCONSULTAS (Mínimo 4)<br>
     a) Criar minimo 1 envolvendo GROUP BY
     b) Criar minimo 1 envolvendo algum tipo de junção

># Marco de Entrega 02: Do item 9.2 até o ítem 9.10<br>

### 10 RELATÓRIOS E GRÁFICOS

#### a) análises e resultados provenientes do banco de dados desenvolvido (usar modelo disponível)
#### b) link com exemplo de relatórios será disponiblizado pelo professor no AVA
#### OBS: Esta é uma atividade de grande relevância no contexto do trabalho. Mantenha o foco nos 5 principais relatórios/resultados visando obter o melhor resultado possível.

    

### 11	AJUSTES DA DOCUMENTAÇÃO, CRIAÇÃO DOS SLIDES E VÍDEO PARA APRESENTAÇAO FINAL <br>

#### a) Modelo (pecha kucha)<br>
#### b) Tempo de apresentação 6:40 

># Marco de Entrega 03: Itens 10 e 11<br>
<br>
<br>




### 12 FORMATACAO NO GIT:<br> 
https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
    
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/
#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/

    
### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. <strong>Caso existam arquivos com conteúdos sigilosos<strong>, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário do git "profmoisesomena", para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://www.sis4.com/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")

