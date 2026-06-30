# 🏆 GoalTrip 2026 – Taller Final Bootstrap

Proyecto desarrollado con **Bootstrap 5** para el Taller Final de Html + Bootstrap + Git.
GoalTrip es una agencia de viajes ficticia especializada en paquetes para asistir al
**Mundial de Fútbol 2026** (USA, Canadá y México).

## 🌐 Demo en vivo
[Ver en GitHub Pages](https://johndaviddiax-ai.github.io/taller_final4/)

## 📁 Estructura del proyecto

```
taller4/
├── index.html              
├── README.md
├── assets/
│   └── img/                
└── app/
    ├── login.html          
    ├── registro.html       
    ├── recuperar.html      
    ├── admin.html          
    └── cliente.html       
```

## 🛠️ Tecnologías usadas

- **Bootstrap 5.3.3** (vía CDN)
- **Bootstrap Icons 1.11.3**
- HTML5 semántico
- Único script del proyecto: `bootstrap.bundle.min.js` (sin JavaScript personalizado adicional)

## 📄 Páginas

| Página | Descripción |
|--------|-------------|
| `index.html` | Landing Page con navbar fija (`fixed-top`) con menú hamburguesa, carrusel de 3 imágenes con `carousel-caption` y botones de acción, sección de cards con paquetes y sedes, sección "Por qué GoalTrip", formulario de contacto y footer en columnas |
| `app/login.html` | Inicio de sesión con `form-floating`, checkbox "Recordarme", botón de ancho completo y enlaces a registro/recuperación |
| `app/registro.html` | Registro con grid de campos en filas (`row`, `col-md-6`), checkbox de términos y condiciones |
| `app/recuperar.html` | Recuperación de contraseña con estructura de validación visual de Bootstrap (`is-valid` / `is-invalid`) |
| `app/admin.html` | Dashboard admin con sidebar, 4 tarjetas de métricas, tabla de participantes con badges contextuales y botones de Editar/Eliminar, y modal de Bootstrap con formulario de edición |
| `app/cliente.html` | Dashboard cliente con panel de perfil, resumen de reservas, pestañas (Activas/Historial) y alerta dismissible |

## ✨ Funcionalidades destacadas

- **Navbar con sección Cliente**: dropdown que enlaza a `app/cliente.html`, `app/login.html` y `app/admin.html`.
- **Carrusel** con `carousel-fade`, indicadores y controles de navegación.
- **Modal de Bootstrap** en el panel admin que se abre con el botón "Editar" y muestra un formulario con datos de ejemplo.
- **Sistema de pestañas** (`nav-tabs`) en el panel cliente para alternar entre reservas activas e historial.
- **Alerta dismissible** en el panel cliente recordando subir documentos de viaje.
- **Estructura responsiva completa** usando el Grid System de Bootstrap (`container`, `row`, `col`) en todas las páginas.

## ⚠️ Estado actual / pendientes

Este proyecto utiliza únicamente los componentes nativos de Bootstrap (modales, tabs, dropdowns, collapse, validación visual estática) que funcionan a través de atributos `data-bs-*`, sin scripts personalizados. Por lo tanto, **aún no cuenta con lógica propia en JavaScript**, lo que significa que las siguientes interacciones todavía no son funcionales y quedan como mejora pendiente:

- Validación dinámica y redirección real en `login.html`.
- Mensaje de éxito dinámico al enviar `registro.html`.
- Validación dinámica del correo en `recuperar.html` (actualmente solo están las clases base de Bootstrap, sin comparación real de datos).
- Búsqueda en vivo sobre la tabla de `admin.html`.
- Carga dinámica de datos por fila y guardado de cambios en el modal de edición de `admin.html`.
- Eliminación de filas con confirmación en `admin.html`.
- Cambio de estado de la reserva al pulsar "Pagar ahora" en `cliente.html`.

## 🚀 Despliegue en GitHub Pages

1. Crea un repositorio en GitHub llamado `taller4`
2. Sube todos los archivos manteniendo la estructura de carpetas (`app/`, `assets/img/`)
3. Ve a **Settings → Pages → Branch: main → / (root)**
4. El sitio estará disponible en `https://tu-usuario.github.io/taller4/`

---
*Taller Final – Html + Bootstrap + Git | SENA 2026*
