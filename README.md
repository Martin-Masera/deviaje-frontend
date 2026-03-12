# ✈️ Deviaje — Frontend

Frontend de la plataforma de reservas de viajes **Deviaje**, desarrollada como **Práctica Supervisada UTN-FRC 2025**. Construida con **Angular 18** y arquitectura de componentes standalone, consume APIs externas reales (Amadeus, HotelBeds, MercadoPago) a través de los microservicios backend.
---

## 🛠️ Tecnologías

| Tecnología | Descripción |
|---|---|
| Angular 18 | Framework principal, componentes standalone |
| Bootstrap 5 | Sistema de grilla y utilidades |
| SCSS | Estilos visuales globales y reutilizables |
| Google Charts | Visualización de datos en dashboards |
| Angular Material | Componentes UI adicionales (tooltips, etc.) |
| jsPDF + autotable | Exportación de reportes a PDF |
| SheetJS (XLSX) | Exportación de reportes a Excel |
| MercadoPago SDK | Integración de pagos |
| JWT | Autenticación y control de sesión |

---

## 🔐 Sistema de roles

La aplicación implementa un sistema de cuatro roles con guards y rutas protegidas:

| Rol | Acceso |
|---|---|
| **Guest** | Home, búsqueda de vuelos/hoteles/paquetes, login, registro |
| **Client** | Todo lo anterior + reservas, pagos, perfil, mis reservas |
| **Agente** | Dashboard de agente, gestión de clientes, reservas |
| **Administrador** | Panel completo: usuarios, dashboards, reportes, estadísticas |

## 🔗 Integraciones

El frontend consume los siguientes servicios a través del backend:

- **Amadeus API** — Búsqueda y reserva de vuelos
- **HotelBeds API** — Búsqueda y reserva de hoteles
- **MercadoPago** — Procesamiento de pagos

---

## 📊 Dashboards

Los paneles de administración y agente incluyen gráficos interactivos con **Google Charts**:

- Reservas por tipo (ColumnChart)
- Ingresos en el tiempo (LineChart)
- Top destinos (BarChart)
- Top aerolíneas (BarChart)

Todos los gráficos permiten exportar los datos en formato **PDF** y **Excel**.

---

## 🎨 Convenciones de estilos

- **Bootstrap 5** para estructura, grilla y espaciado
- **SCSS global** para estilos visuales (colores, sombras, tipografías, bordes)

---

## 📦 Repositorios relacionados

| Repositorio                        | Descripción |
|------------------------------------|-----------|
| [deviaje-frontend](https://github.com/Martin-Masera/deviaje-frontend) | Este repositorio (interfaz) |
| [deviaje-bookings-and-payments](https://github.com/Martin-Masera/deviaje-bookings-and-payments) | Microservicio de reservas y pagos |
| [deviaje-searches](https://github.com/Martin-Masera/deviaje-searches) | Microservicio de búsquedas |
| [deviaje-users-and-auth](https://github.com/Martin-Masera/deviaje-users-and-auth) | Microservicio de usuarios y autenticación |
---

## 👨‍💻 Autor

Desarrollado por **Gustavo Martin Masera** como proyecto final de la Tecnicatura en Programación (UTN-FRC).
