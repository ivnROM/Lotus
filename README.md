# PAGINA TIPO BITWARDEN, ver nombre)?

## Idea

Gestor de datos sensibles centralizado en una web, con posibilidades de:

- Almacenar y generar contraseñas para cuentas  
- Almacenar secretos (llaves RSA)

## Objetivos generales

Permitir el acceso rápido (pero seguro) de un conjunto de usuarios, contraseñas, llaves, notas incluso para que cualquier consumidor de este servicio y de una forma que sus datos no se vean vulnerados ni comprometidos siendo que muchas empresas venden información de estos mismos.

## TEMAS A CONSIDERAR

Ciberseguridad:

- Crypto end-to-end: AES-256, key derivation (PBKDF2/Argon2)
- Zero-knowledge architecture: El servidor nunca ve passwords en plaintext
- Secure key management: Master password, key stretching, salt
- Threat modeling: Qué pasa si se compromete el servidor
- Secure communication: HTTPS, certificate pinning

Web Development:

- Frontend crypto: WebCrypto API, encryption en el browser
- Secure storage: IndexedDB encrypted, memory management
- Complex UI: Vault management, auto-fill, password generation
- Multi-platform: Web, browser extension, móvil
- Real-time sync: Encrypted sync entre dispositivos

Características MVP:

- Master password con key derivation
- Vault básico - store/retrieve passwords encriptados
- Password generator
- Secure notes
- Browser extension básica
- Export/import de vaults

Stack técnico:

- Frontend: React + WebCrypto API
- Backend: Node.js/Python para sync
- DB: PostgreSQL (solo metadata encriptada)
- Extension: WebExtensions API




🎯 Mejoras de Responsividad Implementadas:
CSS Responsive (styles.css):

Tipografía fluida con clamp() para que los tamaños se adapten al viewport
Grid flexible usando grid-template-columns: repeat(auto-fit, minmax(250px, 1fr))
Flexbox responsivo para navegación y elementos
Media queries para tablets (768px) y móviles (480px)
Box-sizing: border-box en todos los elementos importantes

Navegación Responsive:

Se adapta de horizontal a vertical en pantallas pequeñas
Los enlaces se centran automáticamente
Espaciado optimizado para touch

Formularios Mejorados:

Inputs y botones con tamaño mínimo de 44px (recomendación de accesibilidad)
Formularios que se apilan correctamente en móvil
Botones que se adaptan al ancho disponible

Tablas Responsive:

Scroll horizontal automático para tablas anchas
Tamaño mínimo definido para evitar colapso
Padding adaptativo según el tamaño de pantalla

Grids de Tarjetas:

Sistema de grid CSS que se ajusta automáticamente
Tarjetas que mantienen proporción en todos los dispositivos
Contenido que se reorganiza verticalmente en móviles

Breakpoints Implementados:

Desktop: > 768px - Layout completo
Tablet: 768px - Ajustes de espaciado y navegación
Mobile: 480px - Layout vertical, elementos apilados

Detalles Técnicos:

Viewport meta tag añadido a todos los HTML
Textos legibles sin zoom en móviles
Botones con área de toque mínima de 44px
Imágenes que se escalan proporcionalmente
Footer sticky que se mantiene en la parte inferior
