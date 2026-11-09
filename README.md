# Armando Pereira — Computer Engineer & Software Developer Portfolio

<div align="center">

  [![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v3-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
  [![WebGL](https://img.shields.io/badge/Graphics-OGL_WebGL-black?style=for-the-badge&logo=webgl&logoColor=white)](https://github.com/oframe/ogl)
  [![License](https://img.shields.io/badge/License-MIT-000000?style=for-the-badge)](LICENSE)

  <p align="center">
    <strong>Portafolio editorial interactivo de alto rendimiento especializado en Gemelos Digitales, Telemetría IoT, Sistemas Embebidos y Cómputo Paralelo / Distribuido.</strong>
  </p>

  <p align="center">
    Desarrollado por <strong><a href="https://github.com/pereiraarmando41-art">Armando Antonio Pereira</a></strong> — Estudiante Avanzado de Ingeniería en Computación (UNLP) & Desarrollador en Laboratorio LINTI.
  </p>

</div>

---

## ✦ Vista General

Este portafolio web personal presenta un diseño estético moderno, minimalista y editorial con animación fluida y soporte gráfico acelerado por hardware. Fue construido combinando micro-interacciones avanzadas, renderizado WebGL, física de scroll interactiva y soporte bilingüe (Español / Inglés).

El sitio destaca la trayectoria académica y profesional de Armando Pereira en la **Universidad Nacional de La Plata (UNLP)** y en la **Práctica Profesional Supervisada (PPS)** en el **Laboratorio LINTI**, exhibiendo proyectos de sistemas distribuidos, desarrollo embebido y modelado ciber-físico.

---

## ✦ Características Clave y Arquitectura Interactiva

### 1. 🌐 Soporte Bilingüe Nativo (ES / EN)
- Selector de idioma dinámico en el encabezado con persistencia de preferencia local (`localStorage`).
- Alternancia de idioma instantánea basada en clases `lang-es` / `lang-en` y atributos de documento `lang`, manteniendo el 100% del maquetado y los saltos de línea editoriales sin recargas de página.

### 2. 🗞️ Encabezado Editorial y Tipografía Metálica
- Tipografía fluida responsiva (`Plus Jakarta Sans`) con efectos de degradado metálico.
- Barra de navegación con indicador de sección activa (`IntersectionObserver`), accesos directos a redes y descarga de CV.
- Menú lateral (Drawer) optimizado para dispositivos móviles.

### 3. 🔍 Canvas Cinético `ScrollExpandMedia` (Sobre Mí)
- Etapa de expansión de tarjeta multimedia controlada por el scroll vertical del usuario.
- Interpolación suave de dimensiones, sombras y desenfoque (efecto unblur en tiempo real) corriendo a 120 FPS sin penalizaciones de reflow.
- Maquetado perimetral con información de disciplina, trayectoria y ubicación en La Plata.

### 4. 🧭 Canvas Espacial de Experiencia Horizontal
- Contenedor sticky que traduce el desplazamiento vertical del usuario en una progresión horizontal a través de la historia profesional y académica.
- Hitos interactivos de la **UNLP** y el **Laboratorio LINTI** con indicadores de fase HUD y botones de salto rápido.
- Compatibilidad accesible para preferencia de movimiento reducido (`prefers-reduced-motion`).

### 5. 🎡 Tambor 3D `WorksWheel`
- Proyección cilíndrica tridimensional en 3D (`rotateX`, `rotateZ`, `translateZ`) para la exploración de proyectos.
- Gestos suaves de arrastre, desplazamiento por rueda de ratón e integración directa con ventanas modales.

### 6. 🌊 `FlexCarousel` (Lente Líquido WebGL / OGL)
- Carrusel interactivo impulsado por **OGL** (motor WebGL ligero) que aplica efectos de refracción líquida y deformación de malla.
- Sistema de acordeón responsivo en las áreas de especialización y navegación por teclado/táctil.

### 7. 🪟 Modales de Inspección de Proyectos y Contacto
- Modales emergentes con efecto glassmorphism (desenfoque de fondo animado).
- Visualización detallada de entregables, métricas clave, tecnologías y enlaces directos a repositorios de GitHub.
- Formulario de contacto integrado con notificaciones Toast flotantes.

---

## ✦ Stack Tecnológico

| Área | Tecnología | Descripción |
|---|---|---|
| **Estructura** | HTML5 Semántico | Marcado optimizado para SEO y accesibilidad |
| **Estilos** | Tailwind CSS v3 | Sistema de diseño minimalista, tipografía y tokens oscuros/claros |
| **Gráficos & WebGL** | [OGL](https://github.com/oframe/ogl) | Motor WebGL ligero para efectos de lente y deformación líquida |
| **Lógica y Movimiento** | JavaScript Vanilla (ES Modules) | Arquitectura modular sin dependencias pesadas de frameworks |
| **Tipografía** | Plus Jakarta Sans | Tipografía moderna cargada desde Google Fonts |
| **Componentes UI** | `flex-carousel`, `works-wheel`, `scroll-expand-media`, `experience-section` | Motores UI propios e independientes |

---

## ✦ Proyectos Destacados

- **Digital Twin & Batería Hidráulica Virtual (LINTI UNLP)**: Prototipo en Python para el modelado dinámico-estocástico y optimización energética de cisternas de 1400 m³ integrando telemetría IoT y parque fotovoltaico.
- **Resolución Paralela del Problema de las N-Reinas**: Solver híbrido en C (`MPI + Pthreads`) con balanceo dinámico de carga, optimización Bitwise Backtrack (poda por simetría de Takaken) y análisis formal de speedup.
- **Sistemas Embebidos ATmega328P**: Repositorio de firmware bare-metal en C (AVR-GCC) que incluye máquinas de estados finitos (MEF), drivers UART/I2C/ADC y simulación en Proteus VSM.
- **Receptor FM Dual con ESP8266**: Prototipo físico de sintonizador doble combinando módulos TEA5767/HEX3653, multiplexor analógico CD4052, potenciómetro digital X9C103S y servidor web.

---

## ✦ Estructura del Proyecto

```bash
/
├── index.html                   # Maquetado principal y estructura del portafolio
├── flex-carousel.js             # Motor de carrusel líquido basado en WebGL / OGL
├── FlexCarousel.css             # Estilos para carruseles y estados interactivos
├── works-wheel.js               # Componente de tambor 3D vertical (WorksWheel)
├── scroll-expand-media.js       # Motor de expansión multimedia en el scroll
├── experience-section.js        # Timeline horizontal espacial de experiencia
├── README.md                    # Documentación del proyecto
└── assets/                      # Imágenes, capturas de proyectos y documento CV PDF

