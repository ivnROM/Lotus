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
