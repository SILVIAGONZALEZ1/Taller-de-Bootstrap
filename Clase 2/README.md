## **Clase 2: Tipografía y Estilos Básicos**  
**Duración:** 2 horas  
**Objetivo:** Aprender a utilizar las clases de Bootstrap para estilizar tipografía, manejar colores, márgenes, espaciado, y personalizar botones.  

---

### **1. Tipografía en Bootstrap (30 minutos)**  
#### **1.1. Títulos y párrafos**  
Bootstrap proporciona clases para estilizar textos rápidamente:  
- **Títulos (`.h1` a `.h6`):**  
  ```html
  <h1 class="h1">Título 1</h1>
  <h2 class="h2">Título 2</h2>
  <h3 class="h3">Título 3</h3>
  <h4 class="h4">Título 4</h4>
  <h5 class="h5">Título 5</h5>
  <h6 class="h6">Título 6</h6>
  ```
- **Parámetros básicos de texto:**  
  ```html
  <p class="lead">Texto destacado en formato más grande.</p>
  <p>Texto estándar de un párrafo en Bootstrap.</p>
  ```

#### **1.2. Alineación de texto**  
Alinea textos con las clases utilitarias de alineación:  
- **Clases comunes:**
  - `text-start`: Alineado a la izquierda (por defecto).  
  - `text-center`: Centrado.  
  - `text-end`: Alineado a la derecha.  
  - Ejemplo:
    ```html
    <p class="text-start">Texto alineado a la izquierda.</p>
    <p class="text-center">Texto centrado.</p>
    <p class="text-end">Texto alineado a la derecha.</p>
    ```

#### **1.3. Colores de texto**  
Bootstrap incluye clases para cambiar el color del texto:  
- Ejemplo de colores predefinidos:  
  ```html
  <p class="text-primary">Texto en azul (primario).</p>
  <p class="text-danger">Texto en rojo (de alerta).</p>
  <p class="text-success">Texto en verde (de éxito).</p>
  ```

---

### **2. Clases utilitarias para márgenes y espaciado (30 minutos)**  
Bootstrap ofrece una forma rápida de manejar márgenes y rellenos con clases utilitarias:  
#### **2.1. Márgenes (`m-*`)**  
- `m`: Aplica márgenes externos.  
- Valores disponibles: `0`, `1`, `2`, `3`, `4`, `5`, y `auto`.  
- Ejemplo:  
  ```html
  <div class="m-3">Margen en todas las direcciones.</div>
  <div class="mt-3 mb-5">Margen superior e inferior.</div>
  ```

#### **2.2. Rellenos (`p-*`)**  
- `p`: Aplica rellenos internos.  
- Ejemplo:  
  ```html
  <div class="p-4 bg-light border">Con relleno interno de 4 unidades.</div>
  ```

#### **2.3. Espaciado automático (`auto`)**  
- Centra elementos horizontalmente usando `mx-auto`.  
  ```html
  <div class="mx-auto" style="width: 200px;">Elemento centrado horizontalmente.</div>
  ```

---

### **3. Botones y Estilos Predeterminados (30 minutos)**  
Bootstrap incluye clases para crear botones estilizados.  
#### **3.1. Botones básicos**  
```html
<button class="btn btn-primary">Primario</button>
<button class="btn btn-secondary">Secundario</button>
<button class="btn btn-success">Éxito</button>
<button class="btn btn-danger">Alerta</button>
```

#### **3.2. Tamaños de botones**  
```html
<button class="btn btn-primary btn-sm">Botón pequeño</button>
<button class="btn btn-primary btn-lg">Botón grande</button>
```

#### **3.3. Botones de solo borde (`outline`)**  
```html
<button class="btn btn-outline-primary">Primario</button>
<button class="btn btn-outline-danger">Alerta</button>
```

---

### **4. Actividad práctica: Diseñar una página estilizada (30 minutos)**  
#### **Instrucciones:**  
1. Crea una página con un encabezado, párrafos y botones utilizando las clases aprendidas.  
2. Agrega colores, márgenes y alineaciones para estilizar tu contenido.  

#### **Ejemplo de código inicial:**  
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Estilos con Bootstrap</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light">
    <div class="container text-center mt-5">
        <h1 class="text-primary">Bienvenido a Bootstrap</h1>
        <p class="lead text-secondary">Este es un ejemplo con tipografía y botones personalizados.</p>
        <div class="mt-4">
            <button class="btn btn-success btn-lg">Éxito</button>
            <button class="btn btn-outline-danger btn-sm">Cancelar</button>
        </div>
    </div>
</body>
</html>
```

---

### **5. Tarea para Casa**
- Diseña una página con los siguientes elementos:  
  - Título principal centrado.  
  - Dos párrafos alineados a la derecha y en colores diferentes.  
  - Tres botones de distintos tamaños y estilos.  
- Lee la sección de **clases utilitarias** en la [documentación oficial de Bootstrap](https://getbootstrap.com/docs/5.3/utilities/spacing/).

---

### **Materiales Adicionales**
- [Documentación oficial de Tipografía](https://getbootstrap.com/docs/5.3/content/typography/).  
- [Documentación de Botones](https://getbootstrap.com/docs/5.3/components/buttons/).  

😊