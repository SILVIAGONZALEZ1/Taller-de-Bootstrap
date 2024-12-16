### Clase 7: Personalización con Bootstrap y Sass

**Objetivo:**  
Aprender a sobrescribir estilos de Bootstrap utilizando CSS o Sass para personalizar diseños y crear temas únicos.

---

#### **Sección 1: Introducción a la Personalización de Bootstrap**
1. **Opciones de personalización:**
   - Uso de clases predeterminadas.
   - Sobrescribir estilos con CSS.
   - Personalización avanzada con Sass.

2. **Instalación de dependencias (para Sass):**
   - Requisitos: Node.js y npm instalados.
   - Instalación de Bootstrap y Sass:
     ```bash
     npm install bootstrap sass
     ```

---

#### **Sección 2: Sobrescribir Estilos con CSS**
1. Crear un archivo `styles.css` en el proyecto.
2. Importar Bootstrap en el archivo HTML antes de los estilos personalizados:
   ```html
   <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
   <link href="styles.css" rel="stylesheet">
   ```
3. Sobrescribir clases específicas:
   - Cambiar el color de fondo de los botones:
     ```css
     .btn-primary {
         background-color: #ff5722;
         border-color: #ff5722;
     }
     ```
   - Cambiar el espaciado general:
     ```css
     body {
         margin: 20px;
     }
     ```

---

#### **Sección 3: Uso de Sass para Personalización**
1. **Configurar un archivo Sass:**
   - Crear un archivo `custom.scss`.
   - Importar Bootstrap:
     ```scss
     @import "node_modules/bootstrap/scss/bootstrap";
     ```

2. **Modificar variables de Bootstrap:**
   - Antes de importar Bootstrap, redefinir variables para personalización:
     ```scss
     $primary: #4caf50; /* Cambiar el color principal */
     $font-family-sans-serif: 'Arial', sans-serif;

     @import "node_modules/bootstrap/scss/bootstrap";
     ```

3. **Compilar Sass a CSS:**
   - Usar el comando de compilación:
     ```bash
     sass custom.scss custom.css
     ```

4. **Incluir el archivo generado en el proyecto:**
   ```html
   <link href="custom.css" rel="stylesheet">
   ```

---

#### **Sección 4: Creación de un Tema Personalizado**
1. Cambiar colores principales, secundarios y de fondo.
2. Personalizar componentes como tarjetas o formularios.
3. Ejemplo de variables comunes:
   ```scss
   $primary: #6c5ce7;
   $secondary: #fd79a8;
   $body-bg: #f5f6fa;
   ```

---

#### **Actividad Práctica: Personalizar un Diseño con Bootstrap**
1. **Objetivo:**  
   Crear una página personalizada que utilice:
   - Un esquema de colores único.
   - Estilos propios en botones, texto y fondo.
   - Sobrescritura de estilos de componentes como tarjetas y formularios.

2. **Pasos:**
   - Configurar un archivo `custom.scss` para sobrescribir estilos.
   - Personalizar las tarjetas y botones.
   - Incluir estilos únicos en la navegación y el pie de página.

3. **Entrega esperada:**  
   - Una página personalizada con un diseño único que muestre la capacidad de sobrescribir y personalizar estilos de Bootstrap. 😊