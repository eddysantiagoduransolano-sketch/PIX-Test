# PIX-Test
Almacenamiento para la prueba PIX 
Descripción del Proyecto
Este proyecto consiste en un robot desarrollado en PIX Studio que automatiza el ciclo de vida de datos de productos. El proceso incluye la extracción de datos desde una API externa, su almacenamiento y gestión en una base de datos Azure SQL, la generación de un análisis estratégico en Excel mediante macros de VBA, y finalmente, el envío de resultados a través de un formulario web.

Componentes Clave:
Extracción de Datos: Consumo de API REST y respaldo local en formato JSON.
Gestión de Base de Datos: Limpieza e inserción de datos en Azure SQL con validación de duplicados.
Análisis Avanzado: Creación de un archivo .xlsm con una Tabla Dinámica automatizada para categorizar productos y calcular promedios de precios.
Automatización Web: Registro de evidencias y entrega del reporte mediante un formulario web.

Pasos para Ejecución
Para ejecutar el robot correctamente, siga estos pasos:
Extracción e Inserción: Se obtendrán los productos y se cargarán en el servidor SQL.
Generación de Reporte: El robot creará el archivo Excel y ejecutará la macro GenerarReporte para crear las estadísticas.
Llenado de Formulario: Se abrirá el navegador, se completarán los campos del colaborador y se subirá el archivo generado.
Captura de Evidencias: El robot guardará la confirmación del envío en la carpeta Output/Evidencias/.

Requisitos o Dependencias
PIX Studio: Plataforma de RPA utilizada para el desarrollo.
Microsoft Excel: Es necesario tener habilitado el "Acceso al modelo de objetos de proyectos de VBA" en el Centro de Confianza.
Conectividad SQL: Acceso al servidor servidor-rpa-eddy en Azure SQL.
Paquetes de PIX:
PIX.Office.Activities (Para manejo de Excel y macros).
PIX.Database.Activities (Para ejecución de queries SQL).
PIX.Web.Activities (Para automatización de navegador).

Enlace del Formulario Usado
El reporte final y la evidencia visual se envían a través del siguiente formulario:

Formulario: (https://docs.google.com/forms/d/e/1FAIpQLSdcjOOzlvsVtrXpG5DETNrwQ2RqrtKC7Q1mwEpRXkvLMqYI0w/viewform)
