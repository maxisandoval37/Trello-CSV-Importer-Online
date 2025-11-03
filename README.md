# Importador de CSV para Trello

Aplicación web estática que convierte archivos CSV en listas y tarjetas dentro de un tablero de Trello. El flujo se ejecuta 100 % en el navegador: las credenciales se guardan de forma local (opcional) y todas las llamadas se hacen directamente a `api.trello.com`.

## Características
- Carga CSV con encabezado `Name,Description,Labels,List`.
- Crea listas que no existan en el tablero seleccionado antes de generar las tarjetas.
- Puede crear etiquetas automáticamente cuando no estén presentes.
- Permite configurar un retardo entre peticiones para evitar rate limits.
- Incluye registro de progreso y modal con aviso de privacidad.

## Requisitos previos
1. Obtener una **API Key** de Trello desde [https://trello.com/app-key](https://trello.com/app-key).
2. Generar un **token personal** otorgando permisos al tablero donde se importarán las tarjetas.
3. Preparar un archivo CSV con el encabezado mencionado. Los saltos de línea `CRLF` o `LF` y los archivos con BOM son compatibles.

## Uso
1. Ingresar a [Trello-CSV-Importer-Online](https://maxisandoval37.github.io/Trello-CSV-Importer-Online/).
2. Completar la API Key y el token personal.
3. Seleccionar el CSV a importar.
4. Presionar **“Cargar tableros”** para obtener la lista de tableros disponibles.
5. Elegir el tablero destino y ajustar el retardo por tarjeta si es necesario.
6. Presionar **“Importar CSV → Trello”** y seguir el estado en el panel de progreso y el registro.

## CSV de ejemplo
El repositorio incluye `trello.csv` como referencia para el formato esperado. Podés duplicarlo y adaptar su contenido a tus necesidades.

## Desarrollo
El proyecto utiliza únicamente HTML, CSS (Tailwind via CDN) y JavaScript plano. Cualquier editor o servidor estático alcanza para modificarlo o servirlo.

## Información Adicional
Para cualquier información adicional o consultas: <maxisandoval98@gmail.com>

Muchas gracias!
