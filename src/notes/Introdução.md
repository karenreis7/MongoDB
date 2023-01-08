# MONGODB & MONGOOSE

## Banco Relacional vs Não Relacional 

* **Relacional**: Forte configuração de tabela, coluna. tem uma forte relação entre tabelas para o funcionamento; 

* Não Relacional: Não são rigorosos quanto a isso, podemos criar colunas quando um dado é inserido; 

# Mongo

* Banco não relacional mais utilizado;
* Dados são inseridos em formato de objeto do tipo (BSON/JSON); 
* Os comandos são métodos em vez de queries; 
* Relações entre entidades; 
* Facilidade de adaptação para diversas linguagens; 

# Principais Entidades

* Database: onde ficam as collections e dados;
* Collections: são as "tabelas", onde inserimos os dados; 
* Documentos: são os dados; 

_Obs: collections podem ser criadas livremente a qualquer momento e não possuem colunas fixas para os dados._ 

# JSON ou BSON

No MongoDB o tipo de document inserido é do tipo BSON, que é uma variação do JSON, porém tem recursos a mais.  