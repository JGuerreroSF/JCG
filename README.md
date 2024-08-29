## LLM  Pruebas
Repositorio clase sistemas inteligentes

# 1. Instalacion

Como primer paso descargamos [Ollama](https://ollama.com/download/linux) de su pagina web, y ejecutamos el siguente comando:

````bash
curl -fsSL https://ollama.com/install.sh | sh
````
# 2. Ejecutar en el servidor

Ejecutar el servidor de API RESET de Ollama con el siguente comando:

````bash
$ ollama serve
````
# 3. Descargar un modelo

En la pagina de ollama descarga un [Modelo](https://ollama.com/library) 

````bash
$ ollama pull tinyllama
````

# 4. realizar un request a la API RESET con sin steam

Para realizar una consulta utilizamos el comando curl como se muestra en el siguiente ejemplo: 

````bash
$ curl http://localhost:11434/api/generate -d '{
  "model": "tinyllama",
  "prompt": "Why is the sky blue?",
  "stream": false
}'
````
# 5. Realizar un re


## Notas

abrir otra terminal ollama-bash

ollama list: mirar que modelos hay descargados

curl: para trabajar apis en terminal
-x post: acccien en ese caso hacer una pregunta
https://localhoat: url o uri
api/generate: accion
Json los datos
 -o salida.md : para que guarde


git add .    (indexa
git commit -m "UPDATED README.md"   (colocar un verbo     comentario cambio
git push -u origin main (toma los cambios y los manda a la rama principal(main))

"options": {
    "temperature": 0
  },

  temperaruta :0 afin a la info 1: creatividad inventarse cosas

  convertir imagen a base 64 