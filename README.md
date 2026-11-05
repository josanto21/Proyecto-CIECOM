# LUMEN-LINK · Proyecto CIECOM 2026

**Propuesta conceptual de un prototipo de comunicación por luz visible para transmitir audio y datos.**

- **Fecha objetivo:** 16 de noviembre de 2026.
- **Presupuesto máximo:** US$80.
- **Presupuesto preliminar de componentes:** US$74 (estimado, no cotizado).
- **Áreas:** electrónica de potencia e industrial, ingeniería de sonido, microprocesadores, teoría de la comunicación y transmisión de datos.

## Ver la presentación

Abrir **[index.html](./index.html)** en cualquier navegador moderno. Es una página independiente, adaptable a móvil, que no necesita instalar paquetes ni conectarse a un servidor.

Incluye:
1. Una representación gráfica de dos estaciones y el canal óptico.
2. Controles para alternar audio y datos, modificar la distancia ilustrada y bloquear el haz.
3. Una explicación breve para presentar la idea al equipo.
4. Arquitectura, aportes por materia, presupuesto preliminar y cronograma.

**Importante:** la animación es ilustrativa. No es una simulación calibrada ni evidencia de que el prototipo físico ya funcione. Los precios y el alcance óptico deben verificarse antes de comprar o presentar resultados.

## Concepto técnico

- **Modo audio:** micrófono → acondicionamiento → driver LED → luz → fotodetector → amplificador → altavoz.
- **Modo datos:** ESP32 transmisor → modulación OOK → LED → fotodetector → umbral → ESP32 receptor → validación de tramas.

Se propone usar el mismo canal óptico en dos modos seleccionables; no se presupone transmisión simultánea.

**Pregunta de investigación:** ¿cómo afectan la distancia y las obstrucciones a la calidad del audio y a la recepción correcta de datos?

## Presentación en vivo

1. Reproducir audio recibido por luz.
2. Interrumpir el haz y observar el efecto.
3. Enviar datos y mostrar resultados de mediciones reales.

**Plan de contingencia:** si el modo digital no está listo, presentar un enlace de audio estable y experimentos cuantitativos. Priorizar seguridad a 5 V y evitar fuentes luminosas peligrosas.

## Publicación web opcional

Para convertir el repositorio en un sitio accesible mediante una URL de GitHub Pages:

1. Abrir **Settings → Pages** del repositorio.
2. En **Build and deployment**, seleccionar **Deploy from a branch**.
3. Elegir **main** y **/(root)**; guardar.
4. Esperar a que GitHub indique la URL publicada.

Esta configuración **no se realiza automáticamente** al subir el archivo HTML.
