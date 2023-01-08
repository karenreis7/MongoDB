# Gerenciamento de Banco de Dados 

###### Modulo 2 

## Comandos Necessários

* Para verificar os bancos de dados do sistema:  
  * **`show dbs`**
* Para criar um Banco de Dados: 
  * `use <namedobanco>`
* Para verificar o banco atual: 
  * `db`
* Comando para inserir uma collection: 
  * `db.collection.insertOne({dados_desejado})`
* Para encontrar um dado, utilizamos o comando: 
  * `find`
* Para filtrar dados desejados, utilizamos o comando: 
  * `db.<collection>.find({palavra_chave})`

_Obs: O banco será inicializado, mas não será registrado enquanto não tiver um dado inserido_


## Função Pretty

Utilizada para retornar dados mais formatos, pode ser adicionada a alguns comandos, é mais utilizado com o comando find.
`.find.pretty()`