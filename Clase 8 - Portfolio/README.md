### Clase 8: Proyecto Final

**Objetivo:**  
Consolidar los conocimientos adquiridos en Bootstrap mediante la creación de un sitio web completo y funcional, implementando componentes, personalización, y diseño responsivo.

---

### **Sección 1: Introducción al Proyecto Final**
1. **Descripción del proyecto:**  
   Crear un sitio web que combine todos los elementos aprendidos:
   - **Navbar**: Navegación funcional y responsiva.
   - **Grid System**: Diseño adaptable para diferentes dispositivos.
   - **Componentes**: Tarjetas, botones, y elementos interactivos como modales o tooltips.
   - **Formularios**: Formulario de contacto o registro.
   - **Multimedia**: Imágenes, carousels, y videos.

2. **Características requeridas:**
   - Diseño estético y coherente.
   - Uso adecuado de personalización (CSS o Sass).
   - Sitio completamente funcional y responsivo.

3. **Organización:**  
   Los alumnos trabajarán individualmente o en pequeños grupos (máximo 3 personas).  

---

### **Sección 2: Desarrollo Guiado del Proyecto**
1. **Paso 1: Estructura inicial del proyecto**
   - Crear una estructura básica del sitio con carpetas como:
     ```
     /css
     /js
     /images
     index.html
     ```
   - Incluir Bootstrap (CDN o local) y un archivo `styles.css` para personalización adicional.

2. **Paso 2: Implementación de los elementos principales**
   - **Encabezado (Navbar):**
     ```html
     <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
         <div class="container-fluid">
             <a class="navbar-brand" href="#">Mi Sitio</a>
             <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                 <span class="navbar-toggler-icon"></span>
             </button>
             <div class="collapse navbar-collapse" id="navbarNav">
                 <ul class="navbar-nav">
                     <li class="nav-item"><a class="nav-link active" href="#">Inicio</a></li>
                     <li class="nav-item"><a class="nav-link" href="#about">Acerca de</a></li>
                     <li class="nav-item"><a class="nav-link" href="#contact">Contacto</a></li>
                 </ul>
             </div>
         </div>
     </nav>
     ```

   - **Diseño con Grid System:**
     Crear una sección con un diseño responsivo:
     ```html
     <div class="container my-5">
         <div class="row">
             <div class="col-md-6">
                 <h2>Acerca de Nosotros</h2>
                 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
             </div>
             <div class="col-md-6">
                 <img src="images/sample.jpg" alt="Imagen de ejemplo" class="img-fluid">
             </div>
         </div>
     </div>
     ```

   - **Componentes:**  
     Incluir tarjetas, botones, y otros elementos interactivos como un modal:
     ```html
     <div class="card mt-4" style="width: 18rem;">
         <img src="images/card.jpg" class="card-img-top" alt="...">
         <div class="card-body">
             <h5 class="card-title">Título</h5>
             <p class="card-text">Descripción breve.</p>
             <a href="#" class="btn btn-primary">Más Información</a>
         </div>
     </div>
     ```

   - **Formulario:**  
     Crear un formulario de contacto:
     ```html
     <form class="mt-4">
         <div class="mb-3">
             <label for="name" class="form-label">Nombre</label>
             <input type="text" class="form-control" id="name" placeholder="Tu nombre">
         </div>
         <div class="mb-3">
             <label for="email" class="form-label">Correo Electrónico</label>
             <input type="email" class="form-control" id="email" placeholder="Tu correo">
         </div>
         <div class="mb-3">
             <label for="message" class="form-label">Mensaje</label>
             <textarea class="form-control" id="message" rows="3"></textarea>
         </div>
         <button type="submit" class="btn btn-primary">Enviar</button>
     </form>
     ```

3. **Paso 3: Revisión grupal**  
   Cada grupo o alumno presenta su trabajo, explicando:
   - Su estructura y diseño.
   - Problemas encontrados y cómo los resolvieron.

---

### **Sección 3: Integración de Bootstrap en Proyectos Reales**
1. **Consejos prácticos:**
   - Uso de CDN vs. instalación local.
   - Cómo integrar Bootstrap en un proyecto más grande.
   - Buenas prácticas de personalización.

2. **Recursos adicionales:**
   - [Documentación oficial de Bootstrap](https://getbootstrap.com)
   - Herramientas como `Bootswatch` para temas predefinidos.

---

### **Sección 4: Evaluación y Retroalimentación**
1. **Evaluación del proyecto:**
   - Cumplimiento de los requisitos.
   - Originalidad y diseño.
   - Funcionalidad y responsividad.

2. **Retroalimentación:**  
   - Comentarios constructivos de los compañeros y el instructor.
   - Recomendaciones para mejorar habilidades de diseño y desarrollo.

---

### **Resultados Esperados:**
Al finalizar la clase, los alumnos tendrán un sitio web completo y funcional, comprendiendo cómo utilizar Bootstrap para proyectos reales. Además, estarán preparados para aplicar Bootstrap en proyectos futuros con un enfoque profesional.😊