# Anuncios activos con resultados

Abre `analisis-arranque.html` y carga el JSON exportado desde el informe privado. El repositorio público contiene la herramienta, sin datos de clientes.

## Selección

Solo anuncios con estado efectivo ACTIVE al corte y objetivo OUTCOME_LEADS. Por defecto se exige al menos 10 leads en el mes seleccionado y CPL mensual de hasta 10.000 CLP. Ambos umbrales son ajustables; el mínimo nunca baja de tres. Los pausados, archivados y anuncios con uno o dos leads mensuales quedan excluidos. Orden: menor CPL mensual. Estos criterios internos no certifican calidad comercial o rentabilidad.

## Gráficos y comparación

Tres gráficos sincronizados: leads acumulados, gasto acumulado y CPL acumulado. Al pasar el puntero o enfocar un punto se muestran fecha, día, leads, gasto, CPL con dos decimales y resultados del día. El selector de día actualiza la tabla y las guías de los tres gráficos. Las líneas se activan desde la leyenda.

Permite alinear desde primera entrega del anuncio o desde inicio del mes, con horizontes de 7, 14 y 30 días. Día 1 incluye el primer día de la ventana. La tabla también muestra primer día con resultado y tiempo hasta diez leads. Las curvas terminan en el corte; el día del corte se marca como parcial. CPL sin leads se muestra ausente.

## Interpretación

El filtro se basa en resultados mensuales; la curva desde lanzamiento puede mostrar otro período histórico. Elegir un mes anterior no reconstruye el estado pasado del anuncio: se mantiene el estado observado al corte. Un día atribuido no acredita la hora real de captura. Los costos incluyen todo el día, y los días de calendario incluyen pausas. Los nombres, creativos y públicos recuperados son actuales; verificar historial antes de atribuir causas. No se hacen cambios en campañas reales.

## Validación

Verificados cálculo mensual, elegibilidad, exclusión de pausados y bajo volumen, acumulados diarios, CPL, ventanas parciales y ausencia de costo con cero leads. En navegador se comprobaron selección inicial, detalle en puntos de días 5 y 14 y cambio de alineación a inicio de mes. El informe es una fotografía sin conexión en vivo.
