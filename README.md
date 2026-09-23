# ICN292-Lab3-Munoz-Cristobal

## ICN292 - Laboratorio 3: Automatización de Procesos con n8n

*   **Estudiante:** Cristóbal Muñoz
*   **RUT:** 21.657.535-0 (Semilla $S = 535$)
*   **Fecha:** Septiembre 2026
*   **Asignatura:** Sistemas de Información para la Gestión (ICN292)
*   **Institución:** Universidad Técnica Federico Santa María

### Contenido del Repositorio

* `ICN292-Lab3-Munoz-Cristobal-triage.json`: Workflow principal de clasificación y enrutamiento con reglas de negocio.
* `ICN292-Lab3-Munoz-Cristobal-emisor.json`: Workflow disparador que genera y transmite las 15 solicitudes de devolución vía Webhook.
* `ICN292-Lab3-Munoz-Cristobal-schedule.json`: Workflow analítico programado para consolidación de métricas diarias y prevención de división por cero. (ATENCIÓN, ESTE ES EL "ICN292-Lab3-Munoz-Cristobal-resumen.json", PERO LO TOMÉ COMO SCHEDULE)

### Instrucciones de Ejecución (Reproducción en n8n)

Para abrir, visualizar y ejecutar estos flujos de trabajo, es necesario importar los archivos JSON dentro de una instancia de n8n siguiendo estos pasos:

1. Ingresa a tu entorno de n8n (local o en la nube) y ve a la sección **Workflows**.
2. Haz clic en el botón **Add workflow** para crear un lienzo en blanco.
3. En la esquina superior derecha, abre el menú de opciones (tres puntos) y selecciona **Import from File**.
4. Carga uno de los archivos `.json` descargados de este repositorio. Repite este proceso creando un nuevo workflow para cada archivo.
5. **Nota operativa:** Para probar la integración, primero debes importar el flujo de **Triaje** y dejarlo activado (interruptor en *Active*) o ejecutando en modo de prueba (*Listen for test event*). Una vez activo, importa el flujo **Emisor** y presiona *Execute Workflow* para disparar el lote de 15 solicitudes hacia el Webhook del triaje.
