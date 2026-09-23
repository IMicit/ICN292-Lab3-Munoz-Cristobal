# ICN292-Lab3-Munoz-Cristobal

## ICN292 - Laboratorio 3: Automatización de Procesos con n8n

*   **Estudiante:** Cristóbal Muñoz
*   **RUT:** 21.657.535-0 (Semilla $S = 535$)
*   **Fecha:** Septiembre 2026
*   **Asignatura:** Sistemas de Información para la Gestión (ICN292)
*   **Institución:** Universidad Técnica Federico Santa María

### Contenido del Repositorio

*   `ICN292-Lab3-Munoz-Cristobal-triage.json`: Workflow principal de clasificación y enrutamiento con reglas de negocio.
*   `ICN292-Lab3-Munoz-Cristobal-emisor.json`: Workflow disparador que genera y transmite las 15 solicitudes de devolución vía Webhook.
*   `ICN292-Lab3-Munoz-Cristobal-schedule.json`: Workflow analítico programado para consolidación de métricas diarias y prevención de división por cero.

### Instrucciones de Uso

Para reproducir estos flujos de trabajo, necesitas tener acceso a una instancia de [n8n](https://n8n.io/). Sigue estos pasos:

1.  Abre tu entorno de n8n.
2.  Ve a la sección "Workflows" y haz clic en "Add workflow".
3.  En el menú superior derecho (tres puntos), selecciona "Import from File" y carga uno de los archivos `.json` de este repositorio.
4.  Repite el proceso para los otros archivos.
5.  Asegúrate de activar (poner en "Active") el flujo `triage` antes de ejecutar el `emisor` para que el Webhook pueda recibir las peticiones.
