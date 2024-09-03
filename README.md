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

  # 6.GROQ

api keys
 
  ````bash
export GROQ_API_KEY=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
 ````

 sacado de View code de groq
  ````bash
curl "https://api.groq.com/openai/v1/chat/completions" \
  -X POST \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer ${GROQ_API_KEY}" \
  -d '{
         "messages": [
           {
             "role": "user",
             "content": ""
           }
         ],
         "model": "llama3-8b-8192",
         "temperature": 1,
         "max_tokens": 1024,
         "top_p": 1,
         "stream": true,
         "stop": null
       }'
 ````

   ````bash
curl "https://api.groq.com/openai/v1/chat/completions" \
  -X POST \nt-Type: application/json" \
  -H "Content-Type: application/json" \KEY}" \
  -H "Authorization: Bearer ${GROQ_API_KEY}" \
  -d '{  "messages": [
         "messages": [
           { "role": "user",
             "role": "user",r que el cielo es azul?"
             "content": "¿por que el cielo es azul?"
           }
         ],odel": "llama3-8b-8192",
         "model": "llama3-8b-8192",
         "stream": false
         "stream": false
       }'
 ````
