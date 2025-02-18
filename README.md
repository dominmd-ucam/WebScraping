# Web Scraping Tool

## Descripción

Esta herramienta permite a los usuarios extraer información de una página web utilizando XPath. Se desarrolla en **HTML, JavaScript y Tailwind CSS** y permite obtener datos de una URL ingresada por el usuario.

---

## 📌 Requisitos

### **Frontend (HTML, JavaScript y Tailwind CSS)**

- Formulario con dos campos:
  - **URL**: Ingresar la URL de la página web a analizar.
  - **XPath**: Ingresar el XPath para extraer elementos del HTML obtenido.
- Un botón **"Realizar Scraping"** que ejecuta la lógica de scraping.
- Mostrar los resultados en formato de lista o tabla.
- Interfaz atractiva y responsiva usando **Tailwind CSS**.

### **Lógica de Scraping (JavaScript en el Cliente)**

- **Uso de **`` para obtener el HTML de la URL proporcionada.
- **Aplicación de XPath** usando `document.evaluate()`.
- **Ejecución asíncrona** para evitar bloqueos en la interfaz.
- **Manejo de errores** si la URL es inválida o el XPath no devuelve resultados.

---

## 🛠 Instalación y Configuración

### 1️⃣ **Clonar el repositorio**

```bash
  git clone https://github.com/tu-usuario/nombre-del-repo.git
  cd nombre-del-repo
```

### 2️⃣ **Instalar Tailwind CSS**

```bash
  npm install -D tailwindcss
  npx tailwindcss init
```

### 3️⃣ **Configurar Tailwind CSS**

Editar el archivo ``:

```js
module.exports = {
  content: ["./*.html"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

### 4️⃣ **Incluir Tailwind en el CSS**

Crear un archivo `` y agregar:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### 5️⃣ **Generar el CSS de Tailwind**

```bash
  npx tailwindcss -i ./styles.css -o ./output.css --watch
```

### 6️⃣ **Abrir el archivo HTML en el navegador**

Simplemente abre el archivo `index.html` en el navegador para probar la aplicación.

---

## 🚀 Despliegue en GitHub Pages

### 1️⃣ **Subir el código al repositorio**

```bash
  git add .
  git commit -m "Initial commit"
  git push origin main
```

### 2️⃣ **Activar GitHub Pages**

1. Ir a **Configuración** en tu repositorio de GitHub.
2. Buscar la sección **Pages**.
3. Seleccionar la rama `main` y la carpeta `/root`.
4. Guardar y esperar unos minutos para que la página esté disponible.

### 3️⃣ **Acceder a la URL**

La aplicación estará accesible en:

```
https://tu-usuario.github.io/nombre-del-repo/
```

---

## 📩 Contacto

Si tienes preguntas o mejoras, puedes contribuir en el repositorio o contactarme a través de GitHub.

🎯 **Happy Scraping! 🚀**

