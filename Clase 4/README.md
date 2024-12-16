### **Clase 4: Formularios y Controles**  
**Duración:** 2 horas  
**Objetivo:** Aprender a diseñar formularios estilizados y responsivos con Bootstrap, incluyendo validación, controles avanzados y componentes adicionales como dropdowns, checkboxes y radios.  

---

## **1. Clases y Estilos para Formularios (30 minutos)**  

### **1.1. Formularios Básicos**  
- **Estructura básica:**
  ```html
  <form>
      <div class="mb-3">
          <label for="email" class="form-label">Correo Electrónico</label>
          <input type="email" class="form-control" id="email" placeholder="nombre@ejemplo.com">
      </div>
      <div class="mb-3">
          <label for="password" class="form-label">Contraseña</label>
          <input type="password" class="form-control" id="password" placeholder="Contraseña">
      </div>
      <button type="submit" class="btn btn-primary">Enviar</button>
  </form>
  ```

- **Clases útiles:**
  - `form-control`: Da estilo a los inputs y selects.  
  - `form-label`: Estiliza etiquetas.  
  - `form-text`: Agrega texto explicativo o de ayuda debajo de los inputs.

---

### **1.2. Grupos de Entrada (Input Groups)**  
- **Descripción:** Combinación de inputs con elementos adicionales como botones o iconos.  
- **Ejemplo:**  
  ```html
  <div class="input-group mb-3">
      <span class="input-group-text">@</span>
      <input type="text" class="form-control" placeholder="Nombre de usuario">
  </div>
  ```

---

## **2. Elementos Avanzados: Validación y Diseño Responsivo (30 minutos)**  

### **2.1. Validación**  
- **Validación de formularios con clases:** Usa `is-invalid` e `is-valid` para inputs.  
- **Ejemplo:**
  ```html
  <form>
      <div class="mb-3">
          <label for="nombre" class="form-label">Nombre</label>
          <input type="text" class="form-control is-valid" id="nombre" required>
          <div class="valid-feedback">¡Se ve bien!</div>
          <div class="invalid-feedback">Por favor ingresa tu nombre.</div>
      </div>
  </form>
  ```

### **2.2. Formularios Responsivos**  
- **Diseño de columnas para formularios:**  
  ```html
  <form>
      <div class="row g-3">
          <div class="col-md-6">
              <label for="nombre" class="form-label">Nombre</label>
              <input type="text" class="form-control" id="nombre">
          </div>
          <div class="col-md-6">
              <label for="apellido" class="form-label">Apellido</label>
              <input type="text" class="form-control" id="apellido">
          </div>
      </div>
  </form>
  ```

---

## **3. Componentes Adicionales: Dropdowns, Checkboxes y Radios (30 minutos)**  

### **3.1. Dropdowns**  
- **Ejemplo:**  
  ```html
  <div class="dropdown">
      <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown">
          Seleccionar
      </button>
      <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">Opción 1</a></li>
          <li><a class="dropdown-item" href="#">Opción 2</a></li>
      </ul>
  </div>
  ```

### **3.2. Checkboxes y Radios**  
- **Checkboxes:**  
  ```html
  <div class="form-check">
      <input class="form-check-input" type="checkbox" id="terminos">
      <label class="form-check-label" for="terminos">Aceptar términos y condiciones</label>
  </div>
  ```

- **Radios:**  
  ```html
  <div class="form-check">
      <input class="form-check-input" type="radio" name="opciones" id="opcion1">
      <label class="form-check-label" for="opcion1">Opción 1</label>
  </div>
  <div class="form-check">
      <input class="form-check-input" type="radio" name="opciones" id="opcion2">
      <label class="form-check-label" for="opcion2">Opción 2</label>
  </div>
  ```

---

## **4. Actividad Práctica: Formulario de Registro Responsivo (1 hora)**  

### **Instrucciones:**  
1. Diseña un formulario de registro que incluya:  
   - Nombre, Apellido, Email y Contraseña.  
   - Un dropdown para seleccionar el país.  
   - Checkboxes para términos y condiciones.  
   - Radios para opciones de suscripción.  
   - Botón de enviar.  

### **Estructura de ejemplo:**  
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulario de Registro</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <div class="container mt-5">
        <h1 class="text-center">Formulario de Registro</h1>
        <form class="mt-4">
            <div class="row g-3">
                <div class="col-md-6">
                    <label for="nombre" class="form-label">Nombre</label>
                    <input type="text" class="form-control" id="nombre" placeholder="Nombre">
                </div>
                <div class="col-md-6">
                    <label for="apellido" class="form-label">Apellido</label>
                    <input type="text" class="form-control" id="apellido" placeholder="Apellido">
                </div>
            </div>
            <div class="mb-3 mt-3">
                <label for="email" class="form-label">Correo Electrónico</label>
                <input type="email" class="form-control" id="email" placeholder="nombre@ejemplo.com">
            </div>
            <div class="mb-3">
                <label for="password" class="form-label">Contraseña</label>
                <input type="password" class="form-control" id="password" placeholder="Contraseña">
            </div>
            <div class="mb-3">
                <label for="pais" class="form-label">País</label>
                <select class="form-select" id="pais">
                    <option selected>Selecciona tu país</option>
                    <option value="1">México</option>
                    <option value="2">Argentina</option>
                    <option value="3">España</option>
                </select>
            </div>
            <div class="form-check mb-3">
                <input class="form-check-input" type="checkbox" id="terminos">
                <label class="form-check-label" for="terminos">Acepto los términos y condiciones</label>
            </div>
            <button type="submit" class="btn btn-primary">Registrarse</button>
        </form>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

😊