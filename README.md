# Login_Ita

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Objetivo Crear un Login html y documentar su uso en GitHub.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

                  				TECNOLÓGICO NACIONAL DE MEXICO
                  
                               			INSTITUTO TECNOLÓGICO DE OAXACA			
                  
                  			Departamento de Ingeniería en Sistemas Computacionales
                  
                  			Materia: Desarrollo De Software Para La Toma De Decisiones
                     
                  			“Login Enlace de repositorio de Github y/o GitHub Pages”
                  
                  				Profesor: Martinez Nieto Adelina
                  	
                  		Equipo: 
                  			Ramos Jimenéz Xóchitl Itahy
                     
                  		Grupo:   VSI
                  				Oaxaca, Oaxaca, a 03 de julio de 2025.
                      
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
DESCRIPCIÓN: 
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Crear un login base, con css, html con validaciones en correo y cajas de texto.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
¿QUÉ RESUELVE?
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Resulev la necesidad de validar los campos al relleñar formularios validados para el login, aprenddes a comprender mas el codigo css y html.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
COMO ESTA COMPUESTO:
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Esta compuesto por html, css y javaScript para validación. de correos y campos vacios

## 🧾 **Documentación del Proyecto: Login - MotoTribu Scrambler**

### **Estructura general del proyecto**

```plaintext
/ (carpeta raíz)
├── index.html             ← Página de login (este archivo)
├── amotoTribu.html        ← Página principal (a donde se redirige tras iniciar sesión)
├── motos_scrambler2.jpg   ← Imagen mostrada en la portada del login
├── cLogin.css             ← Estilos CSS personalizados
```

### **1. Composición del HTML**

#### `<head>`

Incluye:

* **Bootstrap 5**: Para diseño responsivo y componentes preestilizados.
* **Font Awesome**: Para íconos sociales (Facebook, Google, Twitter, GitHub).
* **cLogin.css**: Estilos personalizados del login.
* **Bootstrap JS**: Para manejar componentes interactivos como los modales o pestañas.

#### `<body>`

Contiene un `section` de altura completa (`vh-100`) con dos columnas principales:

* **Columna Izquierda**: Mensaje de bienvenida e imagen ilustrativa.
* **Columna Derecha**: Pestañas (`nav-pills`) con los formularios de:

  * **Inicio de sesión**
  * **Registro**

### **2. Módulo de Iniciar Sesión**

Incluye:

* Acceso rápido con redes sociales.
* Campos de correo/usuario y contraseña.
* Checkbox para recordar sesión.
* Enlace para recuperar contraseña con **modal**.
* Botón de inicio de sesión con validación.

### **3. Módulo de Registro**

Incluye:

* Campos de nombre, usuario, correo, contraseña y repetir contraseña.
* Aceptación de términos y condiciones.
* Botón para registrarse (no tiene funcionalidad aún).

### **4. Estilos CSS (cLogin.css)**

Se espera que `cLogin.css` contenga personalizaciones visuales como:

* Colores personalizados (botones, fondos, tipografía).
* Alineación de texto y márgenes.
* Adaptaciones responsivas específicas.

> *Puedes agregar ahí sombras, bordes redondeados, efectos hover, etc.*

### **5. JavaScript personalizado**

Ubicado al final del `body`.

#### Funcionalidad del botón **Iniciar sesión**:

```js
document.getElementById("loginButton").addEventListener("click", function (event) {
  event.preventDefault();
  ...
});
```

Este bloque:

* Obtiene el correo y contraseña ingresados.
* Los compara con un usuario de ejemplo:

  * `usuario@ejemplo.com`
  * `123456`
* Si coinciden, redirige a `amotoTribu.html`.
* Si no, muestra un `alert()` con datos de prueba.

####  Funcionalidad para cambiar de pestaña a registro:

```js
document.getElementById('goToRegister').addEventListener('click', function() {
  document.getElementById('pills-register-tab').click();
});
```

Este script hace que al dar clic en **"¿No tienes cuenta?"**, se active la pestaña de registro automáticamente.

### **6. Componentes Bootstrap Utilizados**

* `nav-pills`: para cambiar entre Login / Registro.
* `form-control`: para inputs estilizados.
* `modal`: para recuperación de contraseña.
* `btn`, `btn-primary`, `btn-link`: para botones con estilos predefinidos.
* `row`, `col-md-*`: para diseño responsivo con grid.

### **7. Librerías Externas**

* **Bootstrap CSS & JS** (v5.3.3): `cdn.jsdelivr.net`
* **Font Awesome** (v6.4.2): `cdnjs.cloudflare.com`

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Ejemplo de inicio de sesión:
-------------------------------------------------------------------------------------------------------------------------------------------------------------------

    <script>
    document.getElementById("loginButton").addEventListener("click", function (event) {
      event.preventDefault();
  
      const email = document.getElementById("loginName").value.trim();
      const password = document.getElementById("loginPassword").value.trim();
  
      // Usuario de ejemplo
      const demoEmail = "usuario@ejemplo.com";
      const demoPassword = "123456";
  
      if (email === demoEmail && password === demoPassword) {
        window.location.href = "amotoTribu.html";
      } else {
        alert("Usuario o contraseña incorrectos.\n\nPrueba con:\nUsuario: usuario@ejemplo.com\nContraseña: 123456");
      }
    });
  </script>

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
DEBES INGRESAR CON: 
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
     * `usuario@ejemplo.com`
     * `123456`
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
  ![image](https://github.com/user-attachments/assets/871517df-666c-4e95-adb8-f8fa72379ad7)

  ![image](https://github.com/user-attachments/assets/ffc8338d-9326-48c6-aabd-efc28145fde0)

  ![image](https://github.com/user-attachments/assets/6d76c947-20a8-4c46-a693-bbb7bd4df330)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
![image](https://github.com/user-attachments/assets/f60b33e4-d296-4af4-aed9-e9f39e96d79e)
![image](https://github.com/user-attachments/assets/777dbf27-1c92-4ef5-ae97-aeb4759e3a0a)
![image](https://github.com/user-attachments/assets/36aa0a69-71ef-4dd1-830b-cf97d57e6c4a)
![image](https://github.com/user-attachments/assets/55bcd5f2-c12a-47d2-942a-c4e51764362f)
![image](https://github.com/user-attachments/assets/38b54a33-3223-4eea-93d0-2524ef6f39fd)
![image](https://github.com/user-attachments/assets/bcf29f6e-248d-4719-9bd6-a794edc03c38)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
ENLACE PAGES: 
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
https://itahy.github.io/Login_Ita/cLogin.html?


















                    
