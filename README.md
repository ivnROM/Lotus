# 🪷 Lotus Password Manager

## Concepto

Lotus es un gestor de contraseñas web moderno y seguro, desarrollado como proyecto académico de Ingeniería en Sistemas de Información. Prioriza la privacidad del usuario, la seguridad y una experiencia de usuario intuitiva sin comprometer la protección de datos sensibles.

## Objetivos generales

Permitir el acceso rápido (pero seguro) de un conjunto de usuarios, contraseñas, llaves, notas incluso para que cualquier consumidor de este servicio y de una forma que sus datos no se vean vulnerados ni comprometidos siendo que muchas empresas venden información de estos mismos.

## TEMAS A CONSIDERAR
## Características Principales

### Funcionalidades Core
-  Gestión completa de contraseñas (Crear, Leer, Actualizar, Eliminar)
-  Categorización de contraseñas (Personal, Trabajo, Social, Compras, Entretenimiento)
-  Búsqueda y filtrado en tiempo real
-  Validación de fortaleza de contraseñas
-  Visualización temporal de contraseñas
-  Copiar contraseñas al portapapeles
-  Doble vista: Tabla y Tarjetas
-  Sistema de autenticación con contraseña maestra

### Seguridad
-  Requisitos de contraseña maestra robusta:
  - Mínimo 8 caracteres
  - Al menos una mayúscula
  - Al menos un número
  - Al menos un carácter especial (!@#$%^&*)
-  Indicador visual de fortaleza de contraseña en tiempo real
-  Validación de contraseñas en frontend
-  Almacenamiento local con localStorage (demo)

### Diseño y UX
-  Diseño moderno con tema oscuro y acentos en verde menta (#6ee7b7)
-  Animaciones suaves y transiciones fluidas
-  Interfaz responsive para desktop, tablet y móvil
-  Mensajes toast para feedback del usuario
-  Modales para edición de contraseñas
-  Estados vacíos informativos

## Tecnologías Utilizadas

### Frontend
- **HTML5**: Estructura semántica
- **CSS3**: Estilos modernos con:
  - CSS Grid y Flexbox para layouts
  - Variables CSS para tematización
  - Animaciones y transiciones
  - Media queries para responsive design
- **JavaScript Vanilla**: Lógica del cliente sin dependencias
  - Manipulación del DOM
  - LocalStorage para persistencia
  - Validaciones en tiempo real
  - Event handling

## Responsividad

### Breakpoints
- **Desktop**: > 768px - Layout completo con tabla
- **Tablet**: 768px - Ajustes de espaciado y navegación adaptativa
- **Mobile**: < 768px - Vista de tarjetas optimizada, navegación apilada

### Características Responsive
-  Tipografía fluida adaptable
-  Grids flexibles con `auto-fit` y `minmax()`
-  Navegación que se apila verticalmente en móvil
-  Tablas con scroll horizontal
-  Vista alternativa de tarjetas para móviles
-  Botones con área táctil mínima de 44px
-  Formularios optimizados para touch
-  Viewport meta tag en todos los archivos
