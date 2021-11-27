# EZREST (COPACABANA/FURNAS)

### ESTRUTURA DO PROJETO

- Python 3.9
- PostGreSQL 13

### INSTALAÇÃO DEPENDÊNCIAS

Para instalação das dependências rode o comando:
```
pip install -r requirements.txt
```

### BANCO DE DADOS

Necessário a criação do banco de dados com nome "" para o start do projeto. 
A criação das tabelas e relacionamentos são feitas de forma automática.
Os dados para conexão estão contidos no arquivo __connection.json__ na raiz do projeto.

Exemplo connection.json
```
{
  "DBNAME": "harmonicos",
  "PORT": "5432",
  "USER": "postgres",
  "HOST": "localhost",
  "PASSWORD": "123456"
}

```
### INICIALIZAÇÃO

No terminal, na raiz do projeto, digite o comando abaixo:
```
flask run
```

É possível verificar a documentação do projeto através da URL:

`http://<host:porta>/swagger`


### Rodar as migrations

Na raiz do projeto, rode o comando abaixo:
```
flask db upgrade
```