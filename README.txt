ZAEL ACADEMY — Método de estudio de Ro
=======================================

QUÉ ES
  Mini-app de estudio personal. Quiz interactivo + repaso espaciado,
  con el método de 5 pasos: Escuchar · Elegir · Dibujar · Repetir · Romper.

CÓMO ABRIRLA
  Doble clic en ZAEL-ACADEMY.html. Funciona offline.
  (La 1ª carga de la tipografía y el botón de Google Calendar usan internet;
   sin conexión igual anda todo, solo cambia la fuente.)
  Recomendado: hacele un acceso directo y abrila SIEMPRE desde el mismo
  navegador — tu progreso se guarda ahí (localStorage). Chrome o Edge.

LAS 4 PESTAÑAS
  - El método ...... el ciclo de 5 pasos + reglas anti-overthinking + stack.
  - Quiz ........... elegís módulo → escuchás el resumen (botón 🔊) → quiz.
  - Progreso ....... te dice qué módulo "toca repasar hoy".
  - Ruta a experta . el camino de intermedia a experta en n8n / IA.

CÓMO USAR EL QUIZ
  Tab Quiz → tocás un módulo → leés/escuchás el resumen → "Arrancar quiz".
  Elegís la opción, te corrige al instante y te explica. Al final te da el
  puntaje, los huecos a repasar y un botón para agendar el repaso en
  Google Calendar.

CÓMO AGREGAR UN MÓDULO NUEVO
  Pedile a Claude: "generá el quiz de MX" (M2, M3, ...).
  Claude devuelve un bloque con summary + questions y lo pega en
  ZAEL-ACADEMY.html, reemplazando el slot vacío del módulo.
  Formato detallado en METODO-ESTUDIO.md.

DECISIONES DE DISEÑO (por qué algunas cosas son así)
  - Datos embebidos en el HTML (no data.json aparte): para que abra con
    doble clic sin servidor. Separarlos rompería file:// por CORS. Si algún
    día la subís a un host web, ahí conviene separar data.json.
  - Sin buscador: con 7 módulos no aporta; el selector de módulos alcanza.
  - Estética ZAEL (negro + rojo neón, JetBrains Mono): heredada de tu
    dashboard ZAEL, a propósito. No es ro-brand (eso es para clientes).

VALIDADA CON
  ro-brand · doc-to-app · modo-produccion · pieza-premium (3/6/2026).
  Fixes aplicados: contraste accesible, focus visible, ARIA en tabs,
  animación del feedback del quiz, barra de progreso corregida, copy.

Versión: 1.2 · 3/6/2026
