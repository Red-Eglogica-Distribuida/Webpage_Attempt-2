+++
title = 'Contribuye a la RED'
date = 2026-01-30T07:07:07+01:00
draft = false
showTableOfContents = true
+++



## Contributing


Gracias por tu interés en contribuir a Red Eglógica Distribuida 🌱

Este documento explica cómo preparar el entorno, formatear el código y comprobar que todo funciona correctamente antes de enviar cambios.

⸻

## Requisitos

### Programas instalados
- git
- go
- hugo
Todos ellos open source y gratuítos.


## Instrucciones

### 1. Clonar el repositorio
```bash {class="my-class" id="my-codeblock" lineNos=inline tabWidth=2}
git clone https://github.com/Red-Eglogica-Distribuida/web-page.git
cd red-eglogica
```
⸻

### 2. Hacer las contribuciones deseadas
- Añadir/Modificar el documento en el folder content
  - Posts, si se tratare de un artículo
  - en Wiki, si se tratare de una organización/iniciativa no recogida/alterada.
- En formato markdown,
- con un preámbulo con metadata apropiada
```bash {class="my-class" id="my-codeblock" lineNos=inline tabWidth=2}
+++
title = 'My First Post'
date =  2024-01-14T07:07:07+01:00 (Ejemplo formato fecha.) 
draft = true (cambiar a "false" antes de publicar)
+++
```



⸻

### 3. Comprobar el correcto funcionamiento de los cambios
Ejecutar el comando 'hugo server' en la carpeta del proyecto para ver la página web localmente con los cambios implementados.

⸻

### 4. Presentar los cambios

Hacer un 'pull request' the los cambios con una descripción detallada de los mismos.
⸻

### Scripts disponibles

```bash {class="my-class" id="my-codeblock" lineNos=inline tabWidth=2}
hugo new content content/posts/EXAMPLE.md

hugo server

hugo help


```


## Flujo recomendado

### 1. Crear rama

git checkout -b mi-cambio

### 2. Hacer cambios

### 3. Formatear y validar


### 4. Commit y push

git add .
git commit -m "Describe brevemente el cambio"
git push origin mi-cambio

Luego abre un Pull Request en GitHub.
