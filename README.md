# Encuesta Clínico-Epidemiológica – Síndrome de Guillain-Barré

Formulario web funcional basado en el Anexo 1 del *Hospital Provincial Saturnino Lora*
(Santiago de Cuba). Recoge todos los datos de la encuesta —datos generales, historia
de la enfermedad, epidemiología, manifestaciones clínicas, criterios diagnósticos,
evolución y tratamiento— y **guarda cada encuesta automáticamente como una nueva fila
en un archivo Excel (`encuestas_GBS.xlsx`)**, sin sobrescribir registros anteriores.

## ✨ Características
- Formulario completo con los 74 campos de las secciones I–VII.
- Guardado acumulativo en Excel (Flask + openpyxl) o Google Sheets (Apps Script).
- Multi-usuario: cada envío añade una fila y el formulario queda listo para la siguiente.
- Respaldo en `localStorage` y descarga de pendientes en `.xlsx` si falla la conexión.
- Validación de campos obligatorios y del carné de identidad (11 dígitos).
- Descarga del Excel completo desde `/descargar` para el investigador principal.
