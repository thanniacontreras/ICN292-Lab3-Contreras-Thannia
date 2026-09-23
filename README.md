# ICN292-Lab3-Contreras-Thannia
## Datos del estudiante
*Nombre:* Thannia Contreras Bastidas
*Rut:* 21444986
*Semilla:* 986
*Fecha:* 22/09/2026
## Descripción del proyecto
Este repositorio contiene los archivos desarrollados para el laboratorio 3 de ICN 292. El proyecto automatiza la recepción, evaluación, registro y notificación de solicitudes de devolución mediante workflows creados de n8n.
*El sistema clasifica las solicitudes de acuerdo con las reglas definidas en el laboratorio, registra sus resultados y envía las notificaciones correspondientes.*
## Archivos
- ICN292-Lab3-Contreras-Thannia-triage.json: recibe, valida, clasifica, registra y responde cada solicitud.
- ICN292-Lab3-Contreras-Thannia-emisor.json: envía las 15 solicitudes de prueba al webhook productivo.
- ICN292-Lab3-Contreras-Thannia-resumen.json: genera diariamente el resumen de solicitudes y montos por ruta.
## Instrucciones para reproducir el proyecto en n8n
1. Iniciar sesión en n8n.
2. Crear un workflow nuevo.
3. Abrir el menú de tres puntos ubicado en la parte superior derecha.
4. Seleccionar Import from File.
5. Importar el archivo triage_devoluciones.json.
6. Repetir el procedimiento con los demás archivos .json.
7. Configurar las credenciales de correo, base de datos u otros servicios utilizados.
8. Activar el workflow triage_devoluciones.
9. Copiar la URL de producción del nodo Webhook.
10. Pegar esa URL en el nodo HTTP Request del workflow emisor_solicitudes.
11. Ejecutar el workflow emisor para procesar las solicitudes.
12. Revisar los resultados en el historial de ejecuciones de n8n.
