# Sistema de Gestión de Tickets - Help Desk

Sistema completo de gestión de tickets y clientes tipo help desk con HTML5 y CSS3.

## 📁 Estructura de Archivos

```
html-version/
├── index.html              # Página de login
├── signup.html             # Registro (3 pasos)
├── dashboard.html          # Panel principal
├── tickets.html            # Lista de tickets
├── ticket-detail.html      # Detalle de ticket
├── clients.html            # Lista de clientes
├── client-detail.html      # Detalle de cliente
├── invoices.html           # Lista de facturas
├── invoice-view.html       # ver factura
├── invoice-generate.html   # Generar factura desde ticket
├── invoice-new.html        # Nueva factura (múltiples tickets)
└── styles.css              # Estilos CSS compartidos
```

## 🎨 Características del Diseño

- **Paleta de colores**: 
  - Principal: `#334155` (slate-700)
  - Acción: `#facc15` (amarillo-400)
  - Diseño limpio tipo SaaS

- **Responsive**: Adaptable a móviles y tablets
- **Sidebar fijo**: Navegación lateral con íconos
- **Componentes**: Tarjetas, tablas, formularios, badges, botones

## 🚀 Páginas Implementadas

### 1. **Login (index.html)**
- Formulario de inicio de sesión
- Opción "Recordar sesión"
- Link a recuperar contraseña
- Botón para ir a registro

### 2. **Registro (signup.html)**
- Flujo de 3 pasos con indicador visual
- Paso 1: Información personal
- Paso 2: Datos de empresa
- Paso 3: Verificación y confirmación

### 3. **Dashboard (dashboard.html)**
- 3 tarjetas de estadísticas
- Tabla de tickets recientes
- Botón "Nuevo Ticket"
- Búsqueda de tickets

### 4. **Lista de Tickets (tickets.html)**
- Tabla completa de tickets
- Columnas: ID, Cliente, Tipo de Avería, Estado, Fecha, Acciones
- Estados con badges de colores
- Paginación

### 5. **Detalle de Ticket (ticket-detail.html)**
- Información completa del ticket
- Datos del cliente
- Detalles del equipo
- Información de reparación (diagnóstico, técnico, costos)
- Botones: Ver Cliente, Generar Factura, Volver

### 6. **Lista de Clientes (clients.html)**
- Tabla de clientes con DNI, nombre, teléfono, dirección
- Contador de tickets por cliente
- Búsqueda

### 7. **Detalle de Cliente (client-detail.html)**
- Avatar con iniciales
- Información de contacto
- Lista de tickets del cliente
- Lista de equipos registrados
- Estadísticas (total tickets, equipos)

### 8. **Lista de Facturas (invoices.html)**
- Tabla con: N° Factura, Cliente, Descripción, Base Imponible, IVA, Total, Fecha
- Botón "Nueva Factura"
- Búsqueda

### 9. **Generar Factura desde Ticket (invoice-generate.html)**
- Información del cliente
- Detalles del servicio (ticket)
- Diagnóstico y observaciones
- Cálculo automático: Base imponible, IVA (16%), Total
- Selector de forma de pago

### 10. **Nueva Factura (invoice-new.html)**
- Dropdown para seleccionar cliente
- Tabla con checkboxes para seleccionar múltiples tickets
- Resumen dinámico con cálculo automático
- Validación (botón deshabilitado hasta seleccionar cliente + tickets)

## 🗄️ Datos de Ejemplo

El sistema incluye datos simulados basados en la estructura de base de datos:

- **5 Clientes**: Con DNI, nombres completos, teléfonos, direcciones
- **5 Tickets**: Con tipos de avería variados (pantalla, software, hardware, batería, conectividad)
- **5 Equipos**: Portátiles, PCs, smartphones con sistemas operativos
- **4 Técnicos**: Con especialidades diferentes
- **5 Reparaciones**: Con diagnósticos, costos y observaciones
- **4 Facturas**: Con cálculos de IVA completos

## 💻 Cómo Usar

1. **Abrir en navegador**: Abre `index.html` en cualquier navegador moderno
2. **Navegación**: 
   - Login → Dashboard (automático al enviar)
   - Usar el sidebar para navegar entre secciones
   - Links en tablas para ver detalles
3. **No requiere servidor**: Todo funciona con HTML/CSS/JavaScript puro

## 🎯 Funcionalidades JavaScript

- **Validación de formularios**
- **Navegación entre pasos** (registro)
- **Dropdown interactivo** (selección de clientes)
- **Checkboxes** para selección múltiple de tickets
- **Cálculos automáticos** de subtotal, IVA y totales
- **Actualización dinámica** del resumen de factura

## 📱 Responsive Design

- **Desktop**: Sidebar completo (250px)
- **Tablet**: Sidebar reducido (200px)
- **Mobile**: Sidebar oculto con botón hamburguesa

## 🎨 CSS Features

- **Variables CSS** para colores consistentes
- **Flexbox y Grid** para layouts modernos
- **Transitions** suaves en hover
- **Componentes reutilizables**: `.btn`, `.card`, `.badge`, `.table`
- **Sistema de utilidades**: márgenes, padding, colores de texto

## 🔗 Navegación del Sistema

```
Login → Dashboard
         ├── Tickets → Detalle Ticket → Generar Factura
         ├── Clientes → Detalle Cliente
         └── Facturas → Nueva Factura (múltiples tickets)
```

## ⚙️ Personalización

Para cambiar colores principales, edita en `styles.css`:

```css
/* Colores principales */
.btn-primary { background-color: #facc15; }  /* Amarillo */
.sidebar { background-color: #334155; }      /* Slate */
.btn-secondary { background-color: #334155; }
```

## 📄 Licencia

Código de ejemplo para uso educativo y demostrativo.
