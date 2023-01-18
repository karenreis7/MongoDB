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

* Para mostrar as collectios utilizamos o comando: 
  * `show collections`

* Para remover uma collection utilizamos o comando: 
  * `db.<collection>.drop()`

* Comando para criar um id
  * `db.<collection>.insertOne({ _id:0001, name:"Karen Reis"})`

_Obs: O banco será inicializado, mas não será registrado enquanto não tiver um dado inserido_


## Função Pretty

Utilizada para retornar dados mais formatos, pode ser adicionada a alguns comandos, é mais utilizado com o comando find.
`.find.pretty()`
* O metodo nos retorna um **cursor**; 
* Para receber mais registros, precisamos digitar: it; 
* O cursor **também é um objeto** e possui metodos; 

### Chave Id

<p>Todo o registro no banco vem com uma id, sendo única para todo registro;</p>
<p>O indice ajuda nas consultas pois agiliza o processo;</p> 

