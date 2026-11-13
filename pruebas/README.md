# Prueba de seguimiento de campañas

Descarga `campanas.html` y ábrelo en un navegador moderno. Es un archivo autónomo, sin instalación ni dependencias externas.

Incluye ejemplos simulados de Hyster, Tattersall Multimaq y Ecologic. Todos los números son ficticios y están identificados como tales. No se conecta a plataformas publicitarias ni al CRM.

## Funciones

- Crear y editar campañas, con filtros por cliente y plataforma.
- Ingresar inversión, leads, calificados, fecha de corte y meta interna de CPL calificado.
- Calcular CPL y CPL calificado, distinguiendo falta de resultados de costo cero.
- Hitos internos a los 3, 7, 14 y 30 días, y revisiones semanales posteriores. Registrar una revisión es una acción manual del equipo.
- Registrar último cambio relevante y falla técnica. Los hitos no certifican optimización ni reinician aprendizaje de la plataforma.
- Guardar en el navegador y exportar registros JSON. No hay importación en esta versión.

## Límites

La fecha de evaluación sirve para los hitos; no reconstruye métricas históricas. Los datos con corte posterior se excluyen de los indicadores. Al cambiar el lanzamiento se vacían las revisiones de esa campaña. Las notas y cifras son una fotografía editable, sin historial completo. El almacenamiento es local, no compartido entre usuarios o dispositivos. No ingresar datos personales de prospectos. No modifica campañas reales.

## Validación

14 comprobaciones de lógica ejecutadas con Node: fechas, vencimientos, revisión semanal, costos con cero resultados, cortes futuros y validación de entradas. Sintaxis de ambos scripts verificada. Interfaz pendiente de comprobación visual en navegador.

La propuesta añade archivos en `pruebas/`; mantiene la pantalla existente de avance de diseño.
