# 🎂 Pastelería El Ángel

Sistema web completo desarrollado en PHP y MySQL para la gestión operativa de una pastelería. Permite la administración de productos, pedidos personalizados, usuarios, promociones y stock de insumos, con paneles diferenciados para cliente y administrador.

---

## 🧾 Descripción General

**Pastelería El Ángel** es una solución digital desarrollada como proyecto académico, que simula la operación real de una pastelería:

- Los clientes pueden registrarse, iniciar sesión, personalizar pedidos, visualizar productos y realizar compras.
- Los administradores pueden gestionar productos, actualizar precios, controlar el stock, registrar insumos, activar promociones y monitorear alertas automáticas por stock bajo.

---

## 🧰 Tecnologías Utilizadas

- 💻 **Frontend:** HTML, CSS, JavaScript, formularios y validaciones básicas.
- 🖥️ **Backend:** PHP puro
- 🗃️ **Base de Datos:** MySQL (con phpMyAdmin)
- 🧪 **Servidor local:** XAMPP

---

## 🗂️ Estructura del Proyecto

```
pasteleria_el_angel/
│
├── admin/                   # Panel administrativo
├── css/                     # Estilos personalizados
├── img/                     # Imágenes del sistema
├── includes/                # Archivo de conexión y funciones compartidas
├── js/                      # Scripts del sistema
├── vistas/                 # Interfaz de usuario
├── base_de_datos/           # Scripts y exportaciones de la base de datos
│   ├── pasteleria_el_angel.sql
│   └── script_bd.txt
├── index.php                # Página de inicio
├── perfil_datos.php         # Gestión de perfil de usuario
├── procesar_personalizado.php # Lógica de pedidos personalizados
├── validar_login.php        # Login
├── validar_registro.php     # Registro
├── ver_imagen.php           # Renderizado de imágenes desde la BD
├── .gitignore
└── README.md
```

---

## 🧑‍💼 Roles del sistema

### 👤 Cliente
- Registro e inicio de sesión
- Realizar pedidos personalizados
- Ver historial de pedidos
- Visualizar catálogo de productos

### 👨‍💼 Administrador
- CRUD de productos
- Actualizar stock, precios y estados
- Activar o inactivar productos
- Gestionar insumos y secciones
- Alertas automáticas por stock bajo
- Asignar promociones

---

## 📦 Base de Datos

La base está diseñada en MySQL e incluye relaciones entre productos, insumos, pedidos, usuarios y promociones.

- ✅ `pasteleria_el_angel.sql`: exportación completa desde phpMyAdmin con imágenes en formato binario.
- 📄 `script_bd.txt`: script limpio con estructura de todas las tablas, ideal para consulta rápida o documentación.

### 🧪 Importar base de datos:

1. Abre `http://localhost/phpmyadmin`
2. Crea una base llamada `pasteleria_el_angel`
3. Ve a la pestaña "Importar"
4. Selecciona el archivo `pasteleria_el_angel.sql` ubicado en `base_de_datos/`

---

## 🌐 El proyecto fue desarrollado inicialmente para entorno local (XAMPP) y posteriormente desplegado en un hosting gratuito (InfinityFree) para fines académicos y de demostración.

1. Coloca el proyecto dentro de `C:/xampp/htdocs/`
2. Activa Apache y MySQL desde el panel de XAMPP
3. Abre navegador y visita:  
   `http://localhost/pasteleria_el_angel/`
4. Usa la opción de registro o entra como administrador

---

## 👥 Usuarios del sistema

Este sistema **no incluye usuarios predefinidos públicos**.

### Para comenzar a usar el sistema:
- Regístrate como cliente desde la página principal utilizando el formulario de registro.
- Si deseas utilizar funciones administrativas, crea manualmente un usuario tipo `administrador` desde phpMyAdmin o mediante SQL.

### Ejemplo SQL para crear un administrador:
```sql
INSERT INTO usuarios (nombre, correo, contraseña, tipo_usuario)
VALUES ('Admin', 'admin@angel.com', 'admin123', 'administrador');
```

🔐 Seguridad de contraseñas
Las contraseñas de los usuarios se almacenan utilizando hash seguro con password_hash(), cumpliendo buenas prácticas básicas de seguridad incluso en entorno académico.

---

## 📝 Funcionalidades clave

- ✔️ Autenticación de usuarios (cliente/admin)
- ✔️ Pedidos personalizados con múltiples atributos (sabor, forma, topping...)
- ✔️ Imagen del producto renderizada directamente desde la base
- ✔️ Alertas automáticas por stock mínimo
- ✔️ Panel de administrador funcional y seguro
- ✔️ Activación/inactivación de productos en tiempo real
- ✔️ Promociones y precios dinámicos

---

## 📌 Consideraciones

- Este proyecto fue desarrollado para entorno **local** y no requiere internet.
- Todas las pruebas fueron realizadas en XAMPP v3.3.0
- Para subir a hosting real, bastaría con ajustar las credenciales y migrar la base de datos.

---

## 📤 Autoría

**Desarrollado por:** 

Antonio Izamael 
Angel Israel  
Maria Aurora   


Proyecto académico realizado en 2025 para el curso de Ingeniería de Software.

---

¡Gracias por visitar este repositorio! Para dudas, sugerencias o retroalimentación, no dudes en abrir un issue o contactarme.
