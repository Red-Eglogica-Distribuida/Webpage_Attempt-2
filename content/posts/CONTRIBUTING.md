Contributing

Gracias por tu interés en contribuir a Red Eglógica Distribuida 🌱

Este documento explica cómo preparar el entorno, formatear el código y comprobar que todo funciona correctamente antes de enviar cambios.

⸻

Requisitos
• Node.js ≥ 20
• npm

Se recomienda usar nvm para gestionar versiones de Node:

nvm install 20
nvm use 20

⸻

1. Clonar el repositorio

git clone https://github.com/Red-Eglogica-Distribuida/web-page.git
cd red-eglogica

⸻

2. Instalar dependencias

npm install

Esto instalará las herramientas de desarrollo necesarias (Prettier, html-validate, etc.).

⸻

3. Formatear el código (Prettier)

El proyecto usa Prettier para mantener un estilo consistente.

Qué archivos formatea Prettier
• .css
• .json
• .md
• .yml / .yaml

Formatear automáticamente

npm run format

Comprobar formato (sin modificar archivos)

npm run format:check

⸻

4. Validar HTML

El HTML se valida con html-validate.

npm run html:check

Este comando detecta errores reales de marcado (estructura, atributos inválidos, etc.).

⸻

5. Comprobación de enlaces (CI)

La comprobación de enlaces se ejecuta automáticamente en GitHub Actions mediante Lychee.

En local es opcional y puede hacerse si se tiene Lychee instalado (por ejemplo con Homebrew o Docker).

⸻

Scripts disponibles

Comando Descripción
npm run format Formatea archivos compatibles con Prettier
npm run format:check Comprueba el formato
npm run html:check Valida los archivos HTML

Flujo recomendado

# 1. Crear rama

git checkout -b mi-cambio

# 2. Hacer cambios

# 3. Formatear y validar

npm run format
npm run html:check

# 4. Commit y push

git add .
git commit -m "Describe brevemente el cambio"
git push origin mi-cambio

Luego abre un Pull Request en GitHub.
