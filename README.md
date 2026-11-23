# 🌿 EcoHuella

**HackODS UA 2026 · "Soluciones tecnológicas para retos sociales en Villa El Salvador"**

App móvil de reciclaje responsable que convierte cada botella PET y cada lata de aluminio en **EcoPuntos**, con validación automática por IA.

---

## 👥 Equipo

- **Nombre del equipo:** EcoHuella
- **Líder (contacto con la organización):** Joseph Yerclin Medrano Bautista
- **Integrantes:**
  - Joseph Yerclin Medrano Bautista
  - Kevin Marlon Sánchez de la Cruz

## 📌 Descripción de la solución

**Problema:** en Villa El Salvador el plástico y el aluminio se mezclan con la basura común. Hay pocos puntos de acopio, casi nadie sabe dónde están y reciclar no da ningún beneficio visible.

**Solución:** EcoHuella motiva a reciclar con un flujo simple y verificable:

1. **Encuentra** el punto de acopio más cercano en el mapa.
2. **Escanea** el QR oficial del contenedor (azul = botellas PET, gris = latas de aluminio).
3. **Toma 3 fotos en vivo:** tacho vacío → residuos a reciclar → tacho lleno.
4. **EcoIA valida** la evidencia en unos 4 segundos y acredita los puntos al instante (+10 pts por botella PET, +15 pts por lata).
5. **Canjea** tus EcoPuntos por recompensas.

Si EcoIA tiene dudas, el reporte pasa automáticamente a **revisión manual** de un supervisor.

**Funcionalidades:** mapa de puntos de acopio con ubicación en tiempo real · escáner QR que solo acepta los 2 códigos oficiales · validación por IA (fotos en vivo, calidad, cambio vacío→lleno, reconocimiento y conteo de botellas/latas) · panel de supervisor · historial · impacto (kg reciclados y CO₂ evitado) · niveles y recompensas · modo oscuro.

## 🌍 ODS abordado

- **ODS 12 · Producción y consumo responsables** (principal): incentiva el reciclaje de plástico PET y aluminio.
- **ODS 11 · Ciudades y comunidades sostenibles:** reduce residuos en Villa El Salvador.
- **ODS 13 · Acción por el clima:** mide el CO₂ evitado por cada reciclaje.

_Reto propio, alineado a una problemática real de Villa El Salvador._

## 🛠️ Tecnologías utilizadas

- HTML, CSS y JavaScript (web app móvil)
- Tailwind CSS (diseño) · Leaflet (mapa y ubicación)
- jsQR (lectura de QR con la cámara)
- TensorFlow.js + COCO-SSD (conteo de botellas en el dispositivo)
- EcoIA Cloud, opcional: modelo de visión de Anthropic para reconocer botellas PET y latas

## 🚀 Instrucciones de instalación y uso

**Instalación (no requiere instalar programas)**

1. Descarga el proyecto: en GitHub toca **Code → Download ZIP** y descomprímelo (o usa `git clone https://github.com/medranojosta4-gif/ecohuella.git`).
2. Abre el archivo **`index.html`** con doble clic. Se abrirá en tu navegador (recomendado: Google Chrome) y la aplicación estará lista para usar.
3. Permite el acceso a la **cámara** y a la **ubicación** cuando el navegador lo pida.
4. Se necesita conexión a internet (mapa, lector de QR y reconocimiento de objetos).

**Cómo usarla**

1. Crea tu cuenta (empiezas con 0 EcoPuntos).
2. En **Mapa**, activa tu ubicación para ver los puntos de acopio cercanos.
3. En **Escáner**, apunta la cámara a un cartel QR oficial. Los carteles están en `carteles_qr.html` (QR `ECOHUELLA-AUTONOMA-PET` y `ECOHUELLA-AUTONOMA-LATAS`, los únicos que la app reconoce); imprímelos o ábrelos en otra pantalla.
4. Toma las 3 fotos en vivo y toca **Enviar y Validar con EcoIA**.
5. Revisa tus puntos, tu historial y tu impacto en **Inicio**.

> Los datos de esta demo se guardan en el propio dispositivo (no hay servidor todavía).

## 📈 Impacto esperado y próximos pasos

- Más personas reciclando gracias a un incentivo inmediato.
- Datos reales de kg reciclados y CO₂ evitado por usuario.
- Modelo replicable en otras universidades y distritos de Lima Sur.
- Próximos pasos: base de datos y login real, panel web para supervisores, alianzas para entregar recompensas reales y más puntos de acopio.

## 📄 Licencia

Proyecto académico desarrollado para HackODS UA 2026.
