# 🏆 GoalTrip 2026

**Agencia de viajes ficticia especializada en paquetes turísticos para el Mundial de Fútbol 2026** (USA, Canadá y México).

Proyecto desarrollado para el Taller Final de **Html + Bootstrap + Git** (SENA), construido íntegramente con **Bootstrap 5**, sin CSS personalizado.

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
- Único script del proyecto: `bootstrap.bundle.min.js`, sin JavaScript personalizado adicional

## 📄 Páginas

### `index.html` — Landing Page
Carta de presentación del sitio. Incluye:
- Navbar fija (`fixed-top`) con menú hamburguesa responsivo
- Carrusel (`carousel-fade`) de 3 imágenes con `carousel-caption` y botones de acción
- Banner de estadísticas del torneo (equipos, sedes, partidos, países)
- Sección de cards con paquetes de viaje
- Sección de sedes/destinos
- Sección "¿Por qué GoalTrip?"
- Formulario de contacto con `form-floating`
- Footer oscuro estructurado en columnas

### `app/login.html` — Inicio de sesión
Formulario centrado en card con `form-floating`, campos de correo y contraseña, checkbox "Recordarme", botón de ancho completo (`w-100`) y enlaces a registro y recuperación de contraseña.

### `app/registro.html` — Registro
Formulario extenso organizado con `row` / `col-md-6`: Nombre y Apellidos en una fila, Correo y Teléfono en otra, además de contraseña, país de origen y paquete de interés. Incluye checkbox de aceptación de términos y condiciones.

### `app/recuperar.html` — Recuperación de contraseña
Formulario simple con validación visual estática de Bootstrap (`is-invalid` / `invalid-feedback`) que demuestra cómo se vería un error de "correo no encontrado".

### `app/admin.html` — Dashboard administrativo
Panel con sidebar lateral (oculta en móvil) y:
- 4 tarjetas de métricas clave (Total Inscritos, Ingresos, Reservas Activas, Pendientes) con `badge`
- Tabla de participantes (`table-striped`, `table-hover`, `table-responsive`) con columnas ID, Nombre, Categoría y Estado
- Etiquetas contextuales de estado (Aprobado, Pendiente, Rechazado, En revisión)
- Botones de acción `btn-sm` para Editar y Eliminar
- Modal de Bootstrap con formulario prellenado para editar participantes

### `app/cliente.html` — Dashboard de cliente
Panel con sidebar y:
- Sección de perfil con foto (`rounded-circle`) y datos básicos del usuario
- Tarjetas resumen de reservas, entradas, pagos y próximo partido
- Sistema de pestañas (`nav-tabs`) para alternar entre "Inscripciones Activas" e "Historial"
- Alerta `dismissible` recordando subir documentos de viaje

## ✨ Funcionalidades destacadas

- Navegación completa entre todas las páginas del sitio, incluyendo dropdown "Cliente" en el navbar de la landing page
- Estructura 100% responsiva con el Grid System de Bootstrap (`container`, `row`, `col`) en todas las páginas
- Componentes nativos de Bootstrap activados mediante atributos `data-bs-*` (modales, tabs, dropdowns, alertas dismissibles), sin scripts personalizados

## ⚠️ Estado actual / pendientes

El proyecto utiliza únicamente los componentes nativos de Bootstrap, por lo que aún no cuenta con lógica propia en JavaScript. Quedan como mejora pendiente:

- Validación dinámica y redirección real en `login.html`
- Mensaje de éxito dinámico al enviar `registro.html`
- Validación dinámica del correo en `recuperar.html` (actualmente solo clases base de Bootstrap, sin comparación real de datos)
- Búsqueda en vivo sobre la tabla de `admin.html`
- Carga dinámica de datos y guardado de cambios en el modal de edición de `admin.html`
- Eliminación de filas con confirmación en `admin.html`
- Cambio de estado de la reserva al pulsar "Pagar ahora" en `cliente.html`

## 🚀 Despliegue en GitHub Pages

1. Crea un repositorio en GitHub llamado `taller4`
2. Sube todos los archivos manteniendo la estructura de carpetas (`app/`, `assets/img/`)
3. Ve a **Settings → Pages → Branch: main → / (root)**
4. El sitio estará disponible en `https://tu-usuario.github.io/taller4/`

---
*Taller Final – Html + Bootstrap + Git | SENA 2026*
