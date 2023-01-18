# Crud (Create, Read, Update, Delete)

<p>São as 4 operações basicos de um Banco de Dados.</p>
É onde inserimos, lemos, atualizamos e deletamos dados presentes no banco de dados. 

## Create 

### Document  

É comum adicionar varias entidades com chaves {}

### Relação entre Dados

* Em uma collection não precisamos respietar as chaves dos outros documents; 
* Podemos ter documents totalmente diferentes em uma collection; 

### Inserir varios Dados

* Podemos inserir varios dados atraves do comando: **insertMany**
Sintaxe:
  * `db.<colection>.insertMany({dados})`

* Precisa de uma array e são separados por vírgulas. 
* Configuração que pode ser inserida no insertMany, pode limitar o tempo de execução da inserção:

## Seleção de Dados (Read)

Para encontrar **dados entre valores**, utilizamos o operador $in; 
* Sintaxe:
  * db.collection.find({ categories: {$in: [palavras_chave] }})

obs: para ser encontrados multiplas condições **basta adicionar uma virgula no document** e inserir o proximo requisito. 

* Para encontrar **dados maior que algum valor**, utilizamos o operador: _$gt_ (greater than) 
* Para encontrar **dados menor que algum valor**, utilizamos o operador: _$lt_ (less than) 
* Para resgatar **dados que possuem um valor ou outro**, utilizamos o operador: _$or_. 

Para contar o número de retornos de uma consulta, podemos utilizar o metodo `.count()`

## Atualização de Dados (UPDATE)
Para autlizar um dado utilizamos o método: **updateOne**

* O operador $set é onde ficam os valores a serem atualizados; 
* Primeiros realizamos o filtro e depois inserimos o que precisa ser atualizado; 
Sintaxe: 
  * `db.books.updateOne({ _id: 314}, {$set: { _id: 555}})`

Para atualizar varios itens, usamos o método: **updateMany**
* O update pode servir para adicionar um dado ao document
* Para trocar todos os dados do document utlizamos o método: **replaceOne** \\ hvaerá uma substituição de dados 

* Para adicionar um item a um array utlizamos o operador: **$push**

## Delete

Para deletar usamos o método: **deleteOne**
* Baseado em um filtro, podemos deletar um elemento; 
  `db.books.deleteOne({ _id: 20})`
* Para remover varios arquivos: **deleteMany**
* Para deletar todos os dados de uma collection é só usar o deleteMany sem filtro: `deleteMany()`

