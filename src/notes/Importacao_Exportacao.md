# Importação e Exportação de banco de dados

* Formato mais encontrado é .JSON
* Comando para importar:
  *    `mongoimport<arquivo> -d <database> -c <collection>`
  
Desta maneira é criado um banco de dados nomeado no comando é também uma collection.

* Comando para exportar é: 
  * `mongoexport -c <collection> -d <database> -o <output>`

* Para exportar muitas collections, utilizamos: 
  *  `mongodump -d <nome_banco> -o <diretorio>`

O -o criará uma pasta com os arquivos de cada collections. 

* Importar dados do mongodump:
  * `mongorestore <diretorio>`

### Status do MongoDB

Utilizado para checar informaçãos como: quantidade de consultas, consumo de rede e outros dados; 
* Comando: `mongostat`