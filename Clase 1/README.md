## **Clase 1: Introducción a Bootstrap**
**Duración:** 2 horas  
**Objetivo:** Comprender qué es Bootstrap, cómo instalarlo y aprender a utilizar su sistema de rejilla (Grid System) para crear un diseño responsivo básico.  

---

### **1. Conceptos Básicos (20 minutos)**
#### **¿Qué es Bootstrap?**  
- Bootstrap es una biblioteca de código abierto para diseñar sitios web responsivos y móviles de manera rápida.  
- Ofrece:
  - Un sistema de rejilla flexible.
  - Componentes predefinidos como botones, formularios y menús.
  - Clases utilitarias para espaciado, colores, alineación, etc.  

#### **Ventajas de usar Bootstrap:**  
- Acelera el desarrollo.
- Garantiza consistencia en el diseño.
- Es compatible con navegadores modernos.
- Ideal para diseño responsivo.

#### **Ejemplos de uso:**  
- Sitios web corporativos, tiendas en línea, portfolios personales.

---

### **2. Instalación y Configuración (30 minutos)**
#### **Formas de integrar Bootstrap en tu proyecto:**
1. **CDN (Content Delivery Network):**  
   - Ideal para empezar rápidamente.  
   - Incluye las siguientes líneas en el `<head>` de tu archivo HTML:
     ```html
     <!DOCTYPE html>
     <html lang="en">
     <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Bootstrap Example</title>
       <!-- Bootstrap CSS -->
       <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
     </head>
     <body>
       <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
     </body>
     </html>
     ```

2. **Descarga local:**  
   - Descarga los archivos desde [getbootstrap.com](https://getbootstrap.com).  
   - Guarda los archivos en tu proyecto y enlázalos como cualquier hoja de estilo o script.

3. **Usar un gestor de paquetes:**  
   - Instalar con npm:  
     ```bash
     npm install bootstrap
     ```

#### **Primer archivo HTML con Bootstrap (Actividad guiada):**
- Crea un archivo `index.html`.
- Copia el siguiente código básico:
  ```html
  <!DOCTYPE html>
  <html lang="es">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Mi Primera Página con Bootstrap</title>
      <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  </head>
  <body>
      <h1 class="text-center mt-5">¡Hola, Bootstrap!</h1>
      <p class="text-center">Este es mi primer sitio con diseño responsivo.</p>
  </body>
  </html>
  ```

---

### **3. Sistema de Rejilla (Grid System) (50 minutos)**  
#### **¿Qué es el sistema de rejilla?**  
- Es un sistema basado en 12 columnas para crear diseños responsivos.  
- Permite distribuir contenido en filas y columnas que se adaptan a diferentes tamaños de pantalla.  

#### **Clases principales:**
- **`.container`**: Contenedor principal para centrar el contenido.
- **`.row`**: Define una fila dentro del contenedor.
- **`.col`**: Define una columna en la fila.
  - Ejemplo: `.col-6` ocupa 6 de las 12 columnas.  

#### **Breakpoints en Bootstrap:**  
Bootstrap usa breakpoints para adaptar el diseño:  
- `col-` para dispositivos pequeños.
- `col-sm-`, `col-md-`, `col-lg-`, y `col-xl-` para dispositivos más grandes.

#### **Ejercicio práctico: Crear un diseño básico con rejilla**
1. Copia el siguiente código en tu archivo HTML:
   ```html
   <div class="container">
       <div class="row">
           <div class="col-4 bg-primary text-white text-center">Columna 1</div>
           <div class="col-4 bg-secondary text-white text-center">Columna 2</div>
           <div class="col-4 bg-success text-white text-center">Columna 3</div>
       </div>
   </div>
   ```
2. Modifica las clases para observar cómo cambian las columnas en diferentes tamaños de pantalla.

---

### **4. Actividad Final (20 minutos)**
**Desafío:** Crea una página que incluya:  
1. Un encabezado centrado con Bootstrap.  
2. Una fila con tres columnas de diferentes colores.  
3. Añade márgenes y espaciado utilizando clases utilitarias como `mt-3`, `mb-5`, etc.

---

### **5. Tarea para Casa**
- Lee la documentación oficial sobre el sistema de rejilla: [Documentación de Bootstrap Grid](https://getbootstrap.com/docs/5.3/layout/grid/).  
- Experimenta creando un diseño responsivo con 2 filas y varias columnas.

---

### **Materiales y Recursos**
- [Enlace a la documentación oficial de Bootstrap](https://getbootstrap.com).  
- Plantilla inicial del taller (se puede proporcionar un archivo zip con la estructura básica).  
😊