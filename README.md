# 🏆 GoalTrip 2026 – Taller Final Bootstrap

Proyecto desarrollado con **Bootstrap 5** para el Taller Final de Html + Bootstrap + Git.
GoalTrip es una agencia de viajes ficticia especializada en paquetes para asistir al
**Mundial de Fútbol 2026** (USA, Canadá y México).

## 🌐 Demo en vivo
[Ver en GitHub Pages](https://tu-usuario.github.io/taller4/)

## 📁 Estructura del proyecto

```
taller4/
├── index.html              ← Landing Page principal
├── README.md
├── assets/
│   └── img/                ← Imágenes y logos propios (si se agregan)
└── app/
    ├── login.html          ← Inicio de sesión
    ├── registro.html       ← Registro de usuario
    ├── recuperar.html      ← Recuperar contraseña
    ├── admin.html          ← Dashboard Administrativo
    └── cliente.html        ← Dashboard Cliente/Expositor
```

## 🛠️ Tecnologías usadas

- **Bootstrap 5.3.3** (vía CDN)
- **Bootstrap Icons 1.11.3**
- HTML5 semántico
- Sin CSS personalizado
- JavaScript únicamente con `bootstrap.bundle.min.js` + scripts propios cortos para
  dar funcionalidad real a formularios, modal y tabla (sin frameworks ni librerías externas)

## 📄 Páginas

| Página | Descripción |
|--------|-------------|
| `index.html` | Landing Page con navbar (incluye menú **Cliente**), carrusel, cards de paquetes, sedes, beneficios, contacto y footer |
| `app/login.html` | Inicio de sesión con `form-floating` y validación funcional (campos requeridos + redirección a `cliente.html`) |
| `app/registro.html` | Registro con grid de campos en filas, validación de contraseñas coincidentes y términos obligatorios |
| `app/recuperar.html` | Recuperación con validación visual dinámica `is-valid` / `is-invalid` según el correo ingresado |
| `app/admin.html` | Dashboard admin con sidebar, tabla de participantes, búsqueda en vivo, modal de edición **funcional** (carga y guarda datos reales de cada fila) y eliminación con confirmación |
| `app/cliente.html` | Dashboard cliente con perfil, tabs, alertas y botón **Pagar ahora** que actualiza el estado de la reserva en tiempo real |

## ✨ Funcionalidades destacadas

- **Navbar con sección Cliente**: dropdown que enlaza directamente a `app/cliente.html` y `app/login.html`.
- **Modal de edición real** en el panel admin: cada botón "Editar" carga los datos de su propia fila (no siempre el mismo registro) y al guardar, la tabla se actualiza sin recargar la página.
- **Búsqueda en vivo** en la tabla de participantes.
- **Pago simulado** en el panel cliente: el botón "Pagar ahora" cambia el estado de la reserva de "Pendiente" a "Confirmada" visualmente.
- **Validación de formularios** con la API nativa de validación de Bootstrap (`was-validated`, `checkValidity()`).

## 🚀 Despliegue en GitHub Pages

1. Crea un repositorio en GitHub llamado `taller4`
2. Sube todos los archivos manteniendo la estructura de carpetas (`app/`, `assets/img/`)
3. Ve a **Settings → Pages → Branch: main → / (root)**
4. El sitio estará disponible en `https://tu-usuario.github.io/taller4/`

---
*Taller Final – Html + Bootstrap + Git | SENA 2026*
