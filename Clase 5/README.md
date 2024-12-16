### **Clase 5: Tablas y Multimedia**  
**Duración:** 2 horas  
**Objetivo:** Aprender a estilizar tablas y gestionar elementos multimedia como imágenes y videos usando Bootstrap. Diseñar una página web con una tabla informativa y una galería de imágenes.

---

## **1. Tablas en Bootstrap (30 minutos)**  

### **1.1. Estilización Básica de Tablas**  
Bootstrap proporciona clases para mejorar el diseño y la funcionalidad de las tablas:  
- **Ejemplo básico:**
  ```html
  <table class="table">
      <thead>
          <tr>
              <th scope="col">#</th>
              <th scope="col">Nombre</th>
              <th scope="col">Apellido</th>
              <th scope="col">Correo</th>
          </tr>
      </thead>
      <tbody>
          <tr>
              <th scope="row">1</th>
              <td>Juan</td>
              <td>Pérez</td>
              <td>juanperez@example.com</td>
          </tr>
          <tr>
              <th scope="row">2</th>
              <td>María</td>
              <td>López</td>
              <td>marialopez@example.com</td>
          </tr>
      </tbody>
  </table>
  ```

### **1.2. Clases Adicionales para Tablas**  
- **`table-striped`:** Alterna colores en las filas.  
- **`table-hover`:** Cambia el color de la fila al pasar el cursor.  
- **`table-bordered`:** Añade bordes a las celdas.  
- **Ejemplo:**  
  ```html
  <table class="table table-striped table-hover table-bordered">
      <!-- Contenido de la tabla -->
  </table>
  ```

---

## **2. Gestión de Imágenes (30 minutos)**  

### **2.1. Clases para Tamaño y Adaptabilidad**  
- **Clases importantes:**
  - `img-fluid`: Ajusta la imagen al ancho del contenedor.  
  - `rounded`: Bordes redondeados.  
  - `rounded-circle`: Convierte la imagen en un círculo.  
- **Ejemplo básico:**
  ```html
  <img src="https://via.placeholder.com/300" class="img-fluid rounded" alt="Ejemplo">
  ```

### **2.2. Clases para Alineación**  
- **Clases:**
  - `float-start`: Alinea a la izquierda.  
  - `float-end`: Alinea a la derecha.  
  - `mx-auto d-block`: Centra horizontalmente.  
- **Ejemplo:**  
  ```html
  <img src="https://via.placeholder.com/150" class="float-start" alt="Ejemplo">
  <img src="https://via.placeholder.com/150" class="float-end" alt="Ejemplo">
  ```

---

## **3. Uso de Videos y Elementos Multimedia (30 minutos)**  

### **3.1. Videos Responsivos con Bootstrap**  
- **Ejemplo básico:**
  ```html
  <div class="ratio ratio-16x9">
      <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="Video de YouTube" allowfullscreen></iframe>
  </div>
  ```
- **Clases útiles:**  
  - `ratio-16x9`: Relación de aspecto 16:9.  
  - `ratio-4x3`: Relación de aspecto 4:3.

---

## **4. Actividad Práctica: Página con Tablas y Galería de Imágenes (1 hora)**  

### **Instrucciones:**  
1. Diseña una página que incluya:  
   - Una tabla con información (puedes usar datos ficticios como un inventario o lista de contactos).  
   - Una galería de imágenes en formato de cuadrícula.  
   - Un video incrustado.  

### **Estructura de ejemplo: ver index_5.html**  

---

## **Tarea para Casa**  
- Crea una página similar pero con:  
  - Dos tablas: una para inventario y otra para usuarios registrados.  
  - Una galería con al menos seis imágenes.  
  - Un segundo video de tu elección.  
😊