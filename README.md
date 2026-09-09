Este repositorio contiene componentes Front-End de alto nivel desarrollados para el Instituto Superior YAVIRAC. El objetivo central de este proyecto es demostrar la aplicación rigurosa de **Métricas de Calidad de Software (ISO 25010)** — específicamente en **Usabilidad, Seguridad, Rendimiento y Mantenibilidad** — utilizando exclusivamente tecnologías web nativas (Vanilla JS, HTML5 y CSS3) sin frameworks pesados.
## Componentes del Proyecto
El repositorio está dividido en dos módulos principales, cada uno con características técnicas avanzadas:
### 1. [Módulo de Login Seguro](./LOGIN)
Un sistema de autenticación premium diseñado para prevenir ataques y guiar al usuario.
* **Protección contra Fuerza Bruta:** Sistema de "Lockout" persistente (`localStorage`) que bloquea el formulario por 1 hora tras 3 intentos fallidos.
* **Seguridad Visual:** Popover flotante que valida la complejidad de la contraseña en tiempo real mediante Expresiones Regulares (RegEx).
* **Flujo de Recuperación (Multipasos):** Simulación completa de recuperación de cuenta (OTP de 6 dígitos) con auto-completado inteligente.
### 2. [Módulo de Registro Estudiantil](./FORMULARIO)
Formulario de alta conversión enfocado en la validación estricta de datos en el lado del cliente.
* **Algoritmo Módulo 10 (Cédula Ecuatoriana):** Validación criptográfica oficial en tiempo real del documento de identidad de Ecuador, no solo conteo de 10 dígitos.
* **Sistema Anti-Bots Híbrido (Captcha):** Un mecanismo de dos fases (UI interactiva + Reto visual de cuadrícula) que baraja imágenes dinámicamente con el algoritmo *Fisher-Yates Shuffle*.
* **Micro-interacciones UX:** Feedback inmediato campo por campo y sistema de notificaciones asíncronas (Toasts apilables).
## Arquitectura y Rendimiento (Zero-Bloat)
Al prescindir de librerías como React o Bootstrap, el proyecto garantiza:
* **Performance TTI (Time to Interactive) casi nulo:** Carga instantánea de los recursos.
* **Diseño Mobile-First:** Uso intensivo de CSS Flexbox y Grid, garantizando adaptabilidad desde 360px hasta monitores Ultra-Wide.
* **Mantenibilidad:** Separación estricta de responsabilidades (HTML semántico, CSS de presentación y JS lógico/estado global).
## Tecnologías Utilizadas
* **Lógica y Algoritmos:** `Vanilla JavaScript (ES6+)`
* **Estilos y Animaciones:** `CSS3 (Variables, Keyframes, Glassmorphism)`
* **Estructura Semántica:** `HTML5`
* **Íconos:** `Lucide Icons (CDN)`
## Ejecución Local
Dado que el proyecto está construido con tecnologías nativas del navegador, no requiere instalación de dependencias ni Node.js.
1. Clona el repositorio:
   ```bash
   git clone https://github.com/Skinny420-dev/METRICAS-DEL-SOFTWARE.git
