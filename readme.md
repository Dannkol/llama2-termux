# Instalacion de llama2 en termux android

Instalacion de llama2 en android usando al modelo de 7b, este puede ser cambiado en el archivo installLlama2b.sh pueden buscar modelos en el [huggingface](https://huggingface.co/).

### Pre-Requisitos

* Instalacion de [termux](https://termux.dev/en/).
* Root en equipos que lo necesiten.

## 🛠 Instalacion

Clona el repositorio y ejecuta en la terminal.

```bash
chmod +x installLlama2b.sh
  
./installLlama2b.sh
```

## 💻 Ejecucion

El script ya crea un shortcut para ejecutar el modelo con el ejemplo de prompt Chat_with_bob.

```bash
chat_with_bob_7b
```

si deseas ejecutar un prompt propio o perzonalizado, puedes usar o crear uno dentro de la carpeta ``llama.cpp/prompts`` este seria un ejemplo para un promtp de chat.

```bash
./main -m ./models/{NOMBRE_DEL_MODELO} -n 512 -b 1016 -c 1016 --repeat_penalty 1.0 --color -i -r "{INICIO_CHAT}" -f prompts/{RUTA_PROMPT}
```

* NOMBRE_DEL_MODELO : Nombre del archivo del modelo.
* INICIO_CHAT : Un ejemplo es que si nuestro promtp es para un chat bot, aqui pondriamos un identificador para que el usuario digite su pregunatra por ejemplo ``User:{Query del usuario}``.
* RUTA_PROMPT : Este es el ejemplo de prompt a usar, es como un template que usara el modelo.

Los demas parametros son usados para ajustar varibles como por ejemplo la cantidad de tokens o la predicciones o temperatura, esta puedes encontrarlas ejecutando el comeando.

```bash
./main -h
```
tendras una lista con estas variables y como personalizarlas.

Para terminar recuerda leer la documentacion de [llama.cpp](https://github.com/ggerganov/llama.cpp) para utilizar todo su potencial.

## 🔗 Links

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://dannkol.github.io/portafolios/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/daniel-manosalva-000b98242)

