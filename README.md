# 🚀 NeoAddition - Rediseño Visual & Prototipo Interactivo de Alta Fidelidad

Repositorio oficial con la propuesta de rediseño de interfaz (UI), experiencia de usuario (UX) y arquitectura de componentes para el sitio web corporativo de **NeoAddition** ([https://neoaddition.com/](https://neoaddition.com/)).

Este proyecto respeta y eleva la **paleta de colores institucional original**, soluciona problemas críticos de jerarquía y contacto detectados en la auditoría web, e incorpora componentes interactivos modernos (como el comparador *Before / After* con recorte vectorial y efecto *3D Tilt*).

---

## 🎨 Paleta de Colores Institucional Preservada

Se han mapeado con precisión matemática los colores del Kit Global de Elementor del sitio en producción:

| Color | Código HEX | Rol en la Interfaz | Aplicación |
| :--- | :--- | :--- | :--- |
| **Azul Marino Principal** | `#01055E` | Identidad Corporativa | Encabezados principales, barras de navegación, botones primarios |
| **Azul Medianoche** | `#090246` / `#010441` | Fondos de Alto Contraste | Hero section, franjas tecnológicas y fondo del footer |
| **Cian Neón / Acento** | `#00E8F8` | Interactividad y Conversión | Botones Call-to-Action (CTA), hover states, divisor del slider y badges |
| **Celeste Pastel** | `#A5E0F9` | Soporte y Jerarquía Secundaria | Bordes sutiles, micro-etiquetas y chips |
| **Naranja Melocotón** | `#FFBC7D` | Acento Cálido y Partnerships | Insignia oficial de Creatio y métricas de soporte |
| **Blanco Puro** | `#FFFFFF` | Luminosidad y Legibilidad | Tarjetas sobre fondos claros y textos de alto contraste |
| **Gris Oscuro Sólido** | `#0C1222` | Capa Operación Tradicional | Fondo 100% opaco para la sección comparativa |
| **Gris Carbón** | `#555555` | Cuerpo de Lectura | Párrafos descriptivos corporativos |

---

## 🔍 Diagnóstico y Mejoras Clave Implementadas

### 1. ⚠️ Corrección Crítica en Datos de Contacto
* **Problema:** En el footer del sitio original, el correo de contacto tenía un error tipográfico: `contacto@neoadittion.com` (con doble 't' en lugar de doble 'd'), lo cual causaba el rebote de mensajes de clientes potenciales.
* **Solución:** Corregido de forma global a `contacto@neoaddition.com` con enlace directo y validación visible.

### 2. 🏷️ Jerarquía Semántica W3C & SEO
* **Problema:** Existían 4 etiquetas `<h1>` simultáneas en la portada (`Inicio`, `Somos tu partner...`, `Te ayudamos a optimizar...` y `Testimonios`), perjudicando el posicionamiento orgánico en Google.
* **Solución:** Unificación en un **único `<h1>` semántico estructurado** en el Hero. Las demás secciones se reclasificaron con `<h2>` y `<h3>` lógicos.

### 3. 🎯 Llamadas a la Acción (CTAs) de Alta Conversión
* **Problema:** Ausencia de botones directos de contacto en la cabecera y en el primer pantallazo (*Above the Fold*).
* **Solución:** Inclusión del botón **"Agendar Asesoría"** en la barra sticky y doble botón de conversión en el Hero (**"Iniciar Diagnóstico Gratuito"** en cian neón + **"Explorar Soluciones"**).

### 4. 🎛️ Componente Visual Interactivo (Antes vs. Después)
* **Problema resuelto:** Se diseñó un visualizador interactivo donde el usuario puede arrastrar una barra central para comparar la **Operación Tradicional** (hojas de cálculo, silos, 14 días de retraso) contra la **Operación con NeoAddition** (workflows automáticos ServiceNow/Creatio, 84% de reducción en tiempos de ciclo).
* **Técnica empleada:** Enmascaramiento mediante **CSS `clip-path: polygon(...)`** sobre capas con fondos 100% sólidos, garantizando cero sangrado o superposición de textos en cualquier dispositivo o resolución.
* **Modos de visualización:** 
  1. *Barra Deslizable:* Para interacción fluida por arrastre táctil o ratón.
  2. *Lado a Lado (Side-by-Side):* Comparativa en dos columnas independientes.
* **Selector de 3 escenarios:** ITSM (ServiceNow), CRM (Creatio No-Code) y Gobernanza SMO.

### 5. 💎 Efecto 3D Tilt Parallax
* El mockup tecnológico del Hero calcula en tiempo real la posición del cursor (`mousemove`) para inclinar el panel en tres dimensiones con profundidad realista.

---

## 📂 Estructura del Repositorio

```text
├── index.html                   # Prototipo interactivo completo listo para producción / GitHub Pages
├── prototipo_neoaddition.html   # Copia directa del prototipo de alta fidelidad
├── PLAN_MEJORAS.md              # Documento estratégico con el plan de implementación por fases
├── .gitignore                   # Exclusiones de archivos del repositorio
└── README.md                    # Documentación técnica del proyecto
```

---

## 🛠️ Tecnologías Empleadas

* **HTML5 Semántico:** Cumplimiento de estándares W3C y accesibilidad WCAG 2.1 AA.
* **Tailwind CSS:** Diseño responsivo *mobile-first*, utilidades de espaciado y tokens de diseño.
* **Vanilla JavaScript (ES6+):** Lógica nativa de alto rendimiento sin librerías pesadas externas para el slider, el efecto 3D tilt y el selector de escenarios.
* **Compatibilidad:** 100% responsive (móviles, tablets, pantallas desktop 2K/4K).

---

## 🚀 Despliegue en GitHub Pages

Para publicar este prototipo como un sitio web público interactivo de forma gratuita:
1. Dirígete a la pestaña **Settings** (Configuración) de este repositorio en GitHub.
2. En el menú lateral izquierdo, haz clic en **Pages**.
3. En **Build and deployment > Source**, selecciona la rama `main` y la carpeta `/ (root)`.
4. Haz clic en **Save**. En un par de minutos estará disponible en:
   `https://AlejandraNeo.github.io/neoaddition-redesign/`

---

## 📄 Licencia y Derechos

Propuesta de diseño desarrollada para **NeoAddition**. Todos los derechos reservados © 2026.
