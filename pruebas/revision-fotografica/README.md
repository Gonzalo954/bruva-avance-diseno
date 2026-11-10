# BRÜVA · Prueba de revisión fotográfica

## Cómo probarla

1. Descarga `index.html` de esta carpeta y ábrelo en un navegador moderno. No requiere instalación ni servidor.
2. Pulsa **Probar con ejemplo**, o carga la fotografía original y la editada (JPG, PNG o WebP).
3. Usa **Antes / después** y **Mapa de cambios**. Ajusta la tolerancia si es necesario.
4. Completa la declaración del diseñador y los controles manuales de revisión.
5. Registra una revisión conforme o solicita corrección con observaciones. Descarga el informe JSON para conservar el resultado.

Usa la fotografía editada antes de incorporar textos, logos o composición gráfica. Mantén el mismo encuadre. El ejemplo es una ilustración sintética; no es una fotografía ni evidencia de uso de IA.

## Qué hace

- Compara la diferencia RGB media por píxel sobre una cuadrícula de hasta 640 px de lado mayor.
- Señala diferencias y calcula el área aproximada que supera una tolerancia configurable.
- Informa las dimensiones de ambos archivos.
- Separa el resultado visual de la declaración manual de IA.
- Aplica una regla de marca configurable y exige una referencia de aprobación para cambios de contenido declarados cuando la regla lo requiere.
- Invalida la decisión al cambiar archivos, tolerancia o datos de revisión.
- Exporta un informe JSON sin incluir las fotografías.

## Límites

No es un detector de IA. El porcentaje representa diferencias visuales, nunca una proporción de contenido generado con IA. No hay alineación automática ni reconocimiento de caras. Luz, compresión o desplazamientos pueden producir avisos. Se suspende el porcentaje si las proporciones difieren más de un 2 %.

No inspecciona C2PA. No verifica automáticamente si una declaración es verdadera. La fidelidad de rostros/productos y la nitidez se revisan manualmente en los archivos originales.

Los archivos se procesan en el navegador y no se suben. Sin backend, autenticación ni historial persistente: al recargar se pierde la sesión. El nombre del revisor y las autorizaciones son datos declarados. El registro conforme es solo una prueba del flujo. Las reglas iniciales son ejemplos pendientes de acordar con la marca.

## Validación realizada

- Sintaxis JavaScript verificada con Node.
- Comparación: imágenes idénticas, cambio en la mitad de los píxeles, variaciones bajo el umbral y umbral máximo.
- Navegador: ejemplo, mapa de diferencias, bloqueo por falta de autorización, registro conforme, invalidación al retirar autorización y solicitud de corrección.
- Pendiente de validación con fotografías reales y distintos dispositivos.

El prototipo se agrega en una carpeta separada; no modifica el panel principal de avance de diseño.
