# Manual de Usuario: Configuración de Periodos
## Sistema IKTAN - Gestión de Operaciones Estadísticas

---

## 📋 Tabla de Contenidos

1. [Objetivo](#1-objetivo)
2. [Conceptos Previos](#2-conceptos-previos)
3. [Navegación al Módulo](#3-navegación-al-módulo)
4. [Acceso y Gestión de Periodos](#4-acceso-y-gestión-de-periodos)
5. [Operaciones Principales](#5-operaciones-principales)
6. [Solución de Problemas](#6-solución-de-problemas)

---

## 1. Objetivo

El módulo **Configuración de Periodos** permite administrar los periodos operativos utilizados por los proyectos estadísticos dentro del sistema IKTAN.

### Propósitos Principales:
- Controlar la vigencia de las operaciones
- Asegurar que los dispositivos móviles trabajen con el ciclo operativo correcto
- Mantener sincronización entre oficinas y entidades federativas
- Garantizar integridad de datos operativos

---

## 2. Conceptos Previos

Para utilizar este módulo correctamente, es fundamental entender la siguiente jerarquía de configuración:

### 2.1 Jerarquía de Elementos

| Nivel | Elemento | Descripción | Ejemplo |
|-------|----------|-------------|---------|
| 1 | **Ejercicio** | Año fiscal o de trabajo | 2024, 2025, 2026 |
| 2 | **Calendario** | Define la periodicidad de una encuesta dentro de un ejercicio | "Encuesta ENIGH - Periodicidad Semanal" |
| 3 | **Periodo** | Unidad mínima de tiempo configurada | "Semana 1", "Enero", "Trimestre 1" |

### 2.2 Relación entre Elementos

```
Ejercicio (2024)
    ├── Calendario (ENIGH - Semanal)
    │   ├── Periodo 1 (Semana 1: 01-07 Ene)
    │   ├── Periodo 2 (Semana 2: 08-14 Ene)
    │   └── ...
    └── Calendario (ENOE - Mensual)
        ├── Periodo 1 (Enero)
        ├── Periodo 2 (Febrero)
        └── ...
```

### 2.3 Ámbitos de Aplicación

Los periodos pueden aplicarse en diferentes ámbitos:

- **Ámbito Oficina**: El periodo varía según la oficina que realiza la descarga
- **Ámbito Estatal/Regional**: El periodo se rige por la entidad federativa
- **Ámbito Encuesta**: Periodo general para todo el país

---

## 3. Navegación al Módulo

### 3.1 Ruta de Acceso

Menú Principal → Mantenimiento → Gestión → Encuestas → Configuración de Periodos

**Ruta directa**: `Mantenimiento → Gestión → Encuestas → Configuración de Periodos`

### 3.2 Requisitos de Acceso

- Usuario autenticado en el sistema IKTAN
- Permisos de administración en módulos de configuración
- Acceso a la encuesta/proyecto correspondiente

---

## 4. Acceso y Gestión de Periodos

### 4.1 Filtro de Búsqueda

Una vez en el módulo, utilice los filtros en la parte superior para localizar periodos específicos:

| Campo | Descripción | Notas |
|-------|-------------|-------|
| **Proyecto/Encuesta** | Seleccione el proyecto estadístico correspondiente | Ejemplos: ENIGH, ENOE, ENCASEH |
| **Ejercicio** | Elija el año de trabajo | Solo se muestran ejercicios activos |
| **Calendario** | Si el proyecto cuenta con múltiples calendarios, seleccione el deseado | Ejemplo: mensual y trimestral |

### 4.2 Visualización de la Tabla de Periodos

Una vez configurados los filtros, el sistema muestra la lista de periodos con las siguientes columnas:

| Columna | Tipo | Descripción |
|---------|------|-------------|
| **Consecutivo** | Numérico | Número secuencial que indica el orden del periodo |
| **Título** | Texto | Nombre descriptivo del periodo (ej. "Semana 40") |
| **Tipo de Periodo** | Catálogo | Clasificación: Semana, Mes, Trimestre, etc. |
| **Fecha de Inicio** | Fecha | Inicio del rango operativo |
| **Fecha de Término** | Fecha | Fin del rango operativo |
| **Estatus** | Estado | Activo / Inactivo |

---

## 5. Operaciones Principales

### 5.1 Menú Contextual - Opciones Disponibles

| Opción | Descripción |
|--------|-------------|
| **Modificar** | Edita la información del periodo seleccionado |
| **Eliminar** | Elimina el periodo seleccionado |
| **Consultar** | Visualiza detalles completos del periodo |

⚠️ **Nota**: No se pueden eliminar periodos con avances registrados en campo

### 5.2 Agregar un Nuevo Periodo

**Pasos**:

1. Haga clic en el botón **Agregar**
2. Complete todos los campos requeridos:
   - Consecutivo (número secuencial)
   - Título (nombre descriptivo)
   - Tipo de Periodo
   - Fecha de Inicio
   - Fecha de Término
   - Estatus
3. Haga clic en **Guardar**

### 5.3 Función "Generar Periodos" (Automatización Masiva)

Esta herramienta permite crear automáticamente todos los periodos de un ejercicio completo.

**Pasos**:

1. Seleccione: Proyecto, Ejercicio y Calendario
2. Haga clic en **Generar**
3. Configure:
   - Fecha de Inicio
   - Número de Periodos
   - Prefijo del Título
4. Haga clic en **Aceptar**

---

## 6. Solución de Problemas

### 6.1 Error: "Sin versión disponible"

**Causa**: No existe un periodo configurado o activo

**Solución**:
1. Ingrese al módulo de Configuración de Periodos
2. Verifique que existe un periodo activo
3. Cree uno si es necesario

### 6.2 El Periodo no Aparece en la Tablet

**Causa**: Periodo no guardado o no sincronizado

**Solución**:
- Verifique que presionó "Guardar"
- Sincronice la tablet
- Verifique que el Estatus sea "Activo"

### 6.3 No Puedo Seleccionar el Ejercicio 2026

**Causa**: El ejercicio no existe o no está activo

**Solución**:
- Contacte al administrador del sistema
- El ejercicio debe registrarse en TC_EJERCICIOS

---

## 📝 Información del Documento

| Atributo | Valor |
|----------|-------|
| **Versión** | 2.0 |
| **Sistema** | IKTAN |
| **Módulo** | Configuración de Periodos |
| **Audiencia** | Usuarios finales, Administradores |

---

**© 2026 Sistema IKTAN - Todos los derechos reservados**
