# 🚀 Portfolio de Testing Manual - Universidad Nacional de Hurlingham

## 📂 Documentación Completa
Para ver el detalle técnico completo (hojas de cálculo originales con todos los pasos y precondiciones), podés descargar el archivo fuente haciendo clic en el siguiente enlace o buscándolo en la lista de archivos de este repositorio:

👉 **[Descargar Matriz de Testing (Excel)](./Documentacion-Testing-Manual-Elizabeth-Woca.xlsx)**


Este repositorio contiene la documentación técnica y los reportes de bugs de tres proyectos de práctica profesional, donde se validaron diferentes funcionalidades, lógica de negocio y gestión de errores.

---

## 1. Proyecto: Celfar (Conversor de Temperatura)
Validación de lógica de cálculo (Celsius a Fahrenheit) y manejo de entradas de usuario.
* **Herramientas:** Google Sheets, Metodología Ágil.
* **Bugs Críticos:** Error en el cálculo de temperaturas negativas y enlaces rotos a documentación externa.

### 📋 Casos de Prueba Destacados
| ID | Título | Resultado Esperado | Estado |
|---|---|---|---|
| 1 | Campo numérico modificado | Reemplazar resultado por "Pendiente de cálculo..." | ✅ OK |
| 2 | Límite de caracteres | Mostrar mensaje "El valor ingresado es muy largo" | ❌ Error |
| 3 | Cálculo -17°C | El sistema debe devolver "1.4" | ❌ Error |

---

## 2. Proyecto: Provinciano (Buscador de Provincias)
Testeo de un buscador de provincias argentinas con filtros por región y datos demográficos.
* **Bugs Críticos:** Inversión de datos en las columnas (Habitantes vs Capital) y fallos en la restricción de filtros.

### 📋 Casos de Prueba Destacados
| ID | Título | Resultado Esperado | Estado |
|---|---|---|---|
| 1 | Orden de columnas | Columna "Capital" muestra texto y "Habitantes" números | ❌ Error |
| 2 | Criterio de búsqueda | Al seleccionar "Misiones", solo debe mostrar esa fila | ❌ Error |

---

## 3. Proyecto: Contactos (Gestión de Agenda)
Pruebas sobre una aplicación de gestión de contactos, validando altas, bajas y modificaciones (CRUD).
* **Bugs Críticos:** El sistema permite ingresar números en el campo nombre y falla al intentar editar un nombre existente (detecta email duplicado erróneamente).

### 📋 Casos de Prueba Destacados
| ID | Título | Resultado Esperado | Estado |
|---|---|---|---|
| 1 | Validación de Nombre | Rechazar ingresos numéricos en el campo "Nombre" | ❌ Error |
| 2 | Editar contacto | Permitir modificar el nombre sin dar error de "Email duplicado" | ❌ Error |
