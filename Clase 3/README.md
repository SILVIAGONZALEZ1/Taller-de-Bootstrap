### **Clase 3: Componentes Básicos de Bootstrap**  
**Duración:** 2 horas  
**Objetivo:** Aprender a usar y personalizar componentes esenciales de Bootstrap, como barras de navegación, tarjetas, badges y alerts. Diseñar una página de perfil de usuario usando estos elementos.  

---

## **1. Introducción a los Componentes Básicos (30 minutos)**  

### **1.1. Navbars (Barras de Navegación)**  
- **Descripción:** Las barras de navegación proporcionan menús estructurados para una página web.  
- **Ejemplo básico:**  
  ```html
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-fluid">
          <a class="navbar-brand" href="#">Mi Sitio</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
              <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
              <ul class="navbar-nav">
                  <li class="nav-item">
                      <a class="nav-link active" aria-current="page" href="#">Inicio</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link" href="#">Acerca de</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link" href="#">Contacto</a>
                  </li>
              </ul>
          </div>
      </div>
  </nav>
  ```

---

### **1.2. Cards (Tarjetas)**  
- **Descripción:** Las tarjetas son contenedores flexibles para contenido con opciones de imagen, título y texto.  
- **Ejemplo básico:**  
  ```html
  <div class="card" style="width: 18rem;">
      <img src="https://via.placeholder.com/150" class="card-img-top" alt="...">
      <div class="card-body">
          <h5 class="card-title">Título de la Tarjeta</h5>
          <p class="card-text">Este es un texto breve para describir el contenido de la tarjeta.</p>
          <a href="#" class="btn btn-primary">Leer Más</a>
      </div>
  </div>
  ```

---

### **1.3. Badges y Alerts (Notificaciones)**  
#### **1.3.1. Badges**  
- **Descripción:** Etiquetas pequeñas para resaltar información importante.  
- **Ejemplo:**  
  ```html
  <h1>Notificaciones <span class="badge bg-primary">4</span></h1>
  <button class="btn btn-secondary">
      Mensajes <span class="badge bg-danger">2</span>
  </button>
  ```

#### **1.3.2. Alerts**  
- **Descripción:** Mensajes para mostrar alertas de usuario.  
- **Ejemplo:**  
  ```html
  <div class="alert alert-success" role="alert">
      ¡Acción realizada con éxito!
  </div>
  <div class="alert alert-danger" role="alert">
      Algo salió mal, inténtalo de nuevo.
  </div>
  ```

---

## **2. Personalización Básica de Componentes (30 minutos)**  
- **Colores personalizados:** Modifica la clase para cambiar el color (`bg-primary`, `text-white`, etc.).  
- **Añadiendo iconos:** Usa una biblioteca como [FontAwesome](https://fontawesome.com/) o [Bootstrap Icons](https://icons.getbootstrap.com/).  
  ```html
  <button class="btn btn-primary">
      <i class="bi bi-person"></i> Perfil
  </button>
  ```

---

## **3. Actividad Práctica: Página de Perfil de Usuario (1 hora)**  

### **Instrucciones:**  
1. Diseña una página que incluya:  
   - Una barra de navegación con enlaces (Inicio, Perfil, Configuración).  
   - Una tarjeta de perfil con una imagen, nombre y descripción.  
   - Badges para mostrar notificaciones importantes.  
   - Una alerta al final para mensajes importantes.  

### **Estructura de ejemplo: ver index_3.html**  


## **Tarea para Casa**
- Personaliza la página de perfil para incluir:
  - Un botón que abra un modal (ventana emergente) con información adicional.  
  - Una tarjeta adicional que muestre estadísticas del usuario.  
- Consulta la [documentación de componentes de Bootstrap](https://getbootstrap.com/docs/5.3/components/alerts/) para explorar más opciones.

😊