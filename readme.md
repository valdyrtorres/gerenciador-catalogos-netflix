* Criando um Gerenciador de Catálogos da Netflix com Azure Functions e Banco de Dados em C#
* Bootcamp DIO AZ-204
* Autor: Valdir Torres Borges

O consulta-cards.html mostra como as api's funcionam por meio de uma página html
dependendo da execução as portas podem ser alteradas e modificar o html de acordo assim como os exemplos de chamada abaixo:

* Inclui no storage da azure em um CosmoDB: curl --location 'http://localhost:7217/api/dataStorage' \
--header 'file-type: video' \
--form 'file=@"/C:/Users/valdir/devcode/dio/bootcamp-az-204/gerenciador-catalogos-netflix/handson-serverless-netflix/video.mp4"'
* Inclui filme: curl --location 'http://localhost:7210/api/movie' \
--header 'Content-Type: application/json' \
--data '{
  "id": "a-random-guid-generated", 
  "title": "Harry Potter e o cálice de fogo",
  "year": "2005",
  "video": "https://staflixdiovtbdev001.blob.core.windows.net/video/video.mp4",
  "thumb": "https://staflixdiovtbdev001.blob.core.windows.net/image/thumbvideo.jpg"
}'
* Detalhe do Id: curl --location 'http://localhost:7296/api/detail?id=b5d9c3e9-151a-479b-be06-cf48e815299c'
* Lista todos: curl --location 'http://localhost:7239/api/all'
