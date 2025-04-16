# Tutorial Básico de Banco de Dados

Este repositório tem como objetivo ensinar os conceitos básicos de Banco de Dados, suas operações e suas traduções. Abaixo você encontrará as principais terminologias e comandos usados em SQL, com explicações e exemplos.

## 1. O que é Banco de Dados?

Um banco de dados (BD) é uma coleção de dados organizados de forma estruturada. Eles são usados para armazenar e gerenciar informações de forma eficiente.

## 2. Tabelas

As tabelas são os principais componentes de um banco de dados. Elas armazenam os dados em linhas e colunas, como uma planilha.

**Exemplo de criação de tabela em SQL:**

```sql
CREATE TABLE clientes (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nome VARCHAR(100),
  idade INT,
  email VARCHAR(100)
);
```

### Explicação:
- `CREATE TABLE`: Cria uma nova tabela.
- `id INT AUTO_INCREMENT PRIMARY KEY`: Define uma coluna chamada `id` como chave primária (PRIMARY KEY) que será um número inteiro e aumentará automaticamente a cada novo registro.
- `nome VARCHAR(100)`: Define uma coluna para armazenar o nome com até 100 caracteres.
- `idade INT`: Coluna para armazenar a idade como número inteiro.
- `email VARCHAR(100)`: Coluna para armazenar o email com até 100 caracteres.

## 3. Inserindo Dados

Para inserir dados em uma tabela, usamos o comando `INSERT INTO`.

**Exemplo:**

```sql
INSERT INTO clientes (nome, idade, email) VALUES ('Eric', 18, 'eric@example.com');
```

### Explicação:
- `INSERT INTO`: Comando para inserir dados.
- `clientes`: O nome da tabela onde os dados serão inseridos.
- `nome, idade, email`: As colunas em que os dados serão inseridos.
- `VALUES`: Os valores a serem inseridos nas respectivas colunas.

## 4. Selecionando Dados

Para selecionar e visualizar os dados, usamos o comando `SELECT`.

**Exemplo:**

```sql
SELECT * FROM clientes;
```

### Explicação:
- `SELECT *`: Seleciona todos os dados de todas as colunas.
- `FROM clientes`: Especifica a tabela de onde os dados serão extraídos.

## 5. Atualizando Dados

Se quisermos alterar os dados existentes, usamos o comando `UPDATE`.

**Exemplo:**

```sql
UPDATE clientes SET idade = 19 WHERE nome = 'Eric';
```

### Explicação:
- `UPDATE`: Modifica os dados existentes.
- `SET idade = 19`: Define o novo valor para a coluna `idade`.
- `WHERE nome = 'Eric'`: Aplica a mudança somente aos registros que atendem à condição, neste caso, onde o nome é 'Eric'.

## 6. Deletando Dados

Para remover dados de uma tabela, usamos o comando `DELETE`.

**Exemplo:**

```sql
DELETE FROM clientes WHERE nome = 'Eric';
```

### Explicação:
- `DELETE`: Remove dados da tabela.
- `FROM clientes`: Define de qual tabela os dados serão removidos.
- `WHERE nome = 'Eric'`: Aplica a remoção somente aos registros que atendem à condição.

## 7. Terminologia

Aqui estão algumas traduções e explicações das palavras-chave e comandos mais usados em banco de dados:

| Termo em inglês       | Tradução em português  | Explicação                                                 |
|-----------------------|------------------------|------------------------------------------------------------|
| Database              | Banco de Dados         | Conjunto de dados estruturados armazenados em um sistema.  |
| Table                 | Tabela                 | Estrutura que organiza os dados em linhas e colunas.       |
| Row                   | Linha                  | Registro de dados em uma tabela.                           |
| Column                | Coluna                 | Cada atributo de uma tabela.                               |
| Primary Key           | Chave Primária         | Identificador único para cada registro em uma tabela.      |
| Foreign Key           | Chave Estrangeira      | Coluna que cria uma relação entre duas tabelas.            |
| Query                 | Consulta               | Instrução para consultar ou manipular dados.               |
| SELECT                | SELECIONAR             | Comando para consultar dados de uma tabela.                |
| INSERT INTO           | INSERIR EM             | Comando para inserir dados em uma tabela.                  |
| UPDATE                | ATUALIZAR             | Comando para modificar dados existentes em uma tabela.     |
| DELETE                | DELETAR                | Comando para remover dados de uma tabela.                  |

## 8. Conclusão

Esse tutorial cobriu os conceitos básicos de bancos de dados e SQL. Com esses conhecimentos, você pode começar a trabalhar com bancos de dados relacionais, realizar consultas e manipulações básicas.

Lembre-se de praticar e explorar mais sobre esse universo! O aprendizado contínuo é essencial para um bom domínio.
