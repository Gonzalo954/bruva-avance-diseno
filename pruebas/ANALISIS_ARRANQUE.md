# Análisis del arranque de anuncios

Abre `analisis-arranque.html` en un navegador y carga el JSON exportado desde el informe privado del análisis. El código de este repositorio público no contiene resultados, inversiones ni identificadores de anuncios de clientes.

## Qué muestra

- Días desde primera entrega observada hasta primer día con leads atribuidos.
- Gasto acumulado al cierre de ese día y cantidad de leads atribuidos ese día.
- Leads y CPL en los primeros 3, 7 y 14 días de calendario; marca ventanas incompletas.
- Anuncios sin leads, gasto y días con entrega observada.
- Curvas acumuladas comparables desde día cero, selección de hasta cinco anuncios y filtros por línea, objetivo y resultados.

## Distinciones necesarias

Un día atribuido por Meta no acredita la hora de captura de un formulario. El gasto al cierre de ese día no equivale al gasto exacto hasta el primer lead. Crear un anuncio o programar un conjunto no equivale a comenzar su entrega. Calendario y días con entrega pueden diferir por pausas. Un resultado temprano no acredita maduración ni calidad comercial.

Usar una ventana de atribución consistente y evitar sumar subcategorías de leads que se solapan. La configuración actual del creativo o del público no prueba la configuración histórica del lanzamiento. Validar cambios de creativo y reutilización de IDs antes de atribuir diferencias a un producto.

La cohorte se selecciona por entrega reciente; no constituye un censo de todos los lanzamientos históricos. Los casos sin resultados tienen observación limitada; no son un tiempo de éxito infinito ni cero. Separar objetivos de reconocimiento e interacción de los de captación.

## Validación realizada

Sintaxis JavaScript verificada. Datos del informe reconciliados por ID, fecha, gasto y leads, sin duplicados ID/día. Verificados en navegador: vista inicial, filtros de marca y anuncios sin leads y presencia de curvas SVG. El informe privado usa una fotografía de datos, no una conexión en vivo.
