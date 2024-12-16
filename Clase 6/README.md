### **Clase 6: Diseño Avanzado con Bootstrap**  
**Duración:** 2 horas  
**Objetivo:** Aprender a implementar funcionalidades avanzadas de Bootstrap como menús desplegables (dropdowns), sliders de imágenes (carousels), y elementos interactivos como tooltips y popovers. Diseñar una página con navegación avanzada y un carousel de imágenes.

---

## **1. Menús Desplegables y Navegación Avanzada (30 minutos)**  

### **1.1. Dropdowns (Menús Desplegables)**  
- **Uso básico:**  
  ```html
  <div class="dropdown">
      <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown">
          Menú
      </button>
      <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">Opción 1</a></li>
          <li><a class="dropdown-item" href="#">Opción 2</a></li>
          <li><hr class="dropdown-divider"></li>
          <li><a class="dropdown-item" href="#">Opción 3</a></li>
      </ul>
  </div>
  ```

- **Clases útiles:**
  - `dropdown-menu-end`: Alinea el menú al lado derecho.  
  - `dropdown-item`: Da formato a los elementos del menú.  

### **1.2. Navegación Avanzada**  
- **Barra de navegación con dropdowns:**  
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
                      <a class="nav-link active" href="#">Inicio</a>
                  </li>
                  <li class="nav-item dropdown">
                      <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown">
                          Servicios
                      </a>
                      <ul class="dropdown-menu">
                          <li><a class="dropdown-item" href="#">Servicio 1</a></li>
                          <li><a class="dropdown-item" href="#">Servicio 2</a></li>
                      </ul>
                  </li>
              </ul>
          </div>
      </div>
  </nav>
  ```

---

## **2. Introducción a Carousels (Sliders de Imágenes) (30 minutos)**  

### **2.1. Estructura Básica del Carousel**  
- **Ejemplo:**
  ```html
  <div id="carouselExample" class="carousel slide" data-bs-ride="carousel">
      <div class="carousel-inner">
          <div class="carousel-item active">
              <img src="https://via.placeholder.com/800x400" class="d-block w-100" alt="Imagen 1">
          </div>
          <div class="carousel-item">
              <img src="https://via.placeholder.com/800x400" class="d-block w-100" alt="Imagen 2">
          </div>
          <div class="carousel-item">
              <img src="https://via.placeholder.com/800x400" class="d-block w-100" alt="Imagen 3">
          </div>
      </div>
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Anterior</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Siguiente</span>
      </button>
  </div>
  ```

- **Clases importantes:**
  - `carousel-inner`: Contenedor para las imágenes.  
  - `carousel-item`: Cada imagen o elemento del slider.  
  - `carousel-control-prev` y `carousel-control-next`: Botones para cambiar de imagen.

---

## **3. Tooltip y Popovers (30 minutos)**  

### **3.1. Tooltip**  
- **Descripción:** Muestra información adicional al pasar el cursor sobre un elemento.  
- **Ejemplo:**  
  ```html
  <button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" title="Este es un tooltip">
      Hover para ver tooltip
  </button>
  ```
- **Activación mediante JavaScript:**  
  ```javascript
  var tooltipTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]'));
  var tooltipList = tooltipTriggerList.map(function (tooltipTriggerEl) {
      return new bootstrap.Tooltip(tooltipTriggerEl);
  });
  ```

### **3.2. Popovers**  
- **Descripción:** Similar al tooltip, pero con más contenido y personalización.  
- **Ejemplo:**  
  ```html
  <button type="button" class="btn btn-primary" data-bs-toggle="popover" title="Título" data-bs-content="Contenido del popover">
      Clic para ver popover
  </button>
  ```
- **Activación mediante JavaScript:**  
  ```javascript
  var popoverTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="popover"]'));
  var popoverList = popoverTriggerList.map(function (popoverTriggerEl) {
      return new bootstrap.Popover(popoverTriggerEl);
  });
  ```

---

## **4. Actividad Práctica: Página con Navegación Avanzada y Carousel (1 hora)**  

### **Instrucciones:**  
1. Diseña una página con los siguientes elementos:  
   - Barra de navegación con dropdowns y enlaces.  
   - Carousel con al menos tres imágenes.  
   - Botones con tooltips.  
   - Botón que despliegue un popover.  

### **Estructura de ejemplo:**  
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Diseño Avanzado</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <div class="container mt-5">
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">Mi Sitio</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNav">
                    <ul class="navbar-nav">
                        <li class="nav-item"><a class="nav-link active" href="#">Inicio</a></li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" data-bs-toggle="dropdown">Menú</a>
                            <ul class="dropdown-menu">
                                <li><a class="dropdown-item" href="#">Opción 1</a></li>
                                <li><a class="dropdown-item" href="#">Opción 2</a></li>
                            </ul>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>

        <div id="carouselExample" class="carousel slide mt-4" data-bs-ride="carousel">
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img src="https://via.placeholder.com/800x400" class="d-block w-100" alt="Imagen 1">
                </div>
                <div class="carousel-item">
                    <img src="https://via.placeholder.com/800x400" class="d-block w-100" alt="Imagen 2">
                </div>
                <div class="carousel-item">
                    <img src="https://via.placeholder.com/800x400" class="d-block w-100" alt="Imagen 3">
                </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
                <span class="carousel-control-prev-icon"></span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
                <span class="carousel-control-next-icon"></span>
            </button>
        </div>

        <div class="mt-4">
            <button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" title="Información rápida">Tooltip</button>
            <button type="button" class="btn btn-primary" data-bs-toggle="popover" title="Más Info" data-bs-content="Contenido extendido.">Popover</button>
        </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        var tooltipTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]'));
        tooltipTriggerList.map(function (el) {
            return new bootstrap.Tooltip(el);
        });

        var popoverTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="popover"]'));
        popoverTriggerList.map(function (el) {
            return new bootstrap.Popover(el);
        });
    </script>
</body>
</html>
```
😊