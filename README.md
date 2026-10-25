# DAT-05_ANALISIS_y_Visualizacion_de_Datos-Esumer-Medellin

Repositorio personal de apoyo del curso **Analítica y Visualización de Datos para la Toma de Decisiones** de la universidad ESUMER / Estud-IA. Contiene únicamente el material que tengo recopilado de las clases dictadas hasta el momento: laboratorios guiados en Python, análisis con Pandas y SQL, y un caso progresivo de calidad, transformación, agrupación e integración de datos. No corresponde a todo el contenido de las clases ni al material completo del curso.

> **Importante:** los archivos de matrículas, estudiantes, programas y ventas son datos sintéticos para fines educativos. No representan personas reales ni deben interpretarse como información institucional real.

## Contenido disponible hasta el momento

El material disponible está organizado por clases y puede recorrerse de forma progresiva. Esta lista corresponde únicamente a lo que tengo hasta el momento y no representa todas las clases ni todo lo visto en cada clase:

| Carpeta | Tema principal | Material |
|---|---|---|
| `Clase 3 y 4` | Fundamentos de Python para análisis de datos | Variables, tipos, listas, operadores, condicionales, ciclos y carga de datos |
| `Clase 5` | Pandas aplicado e introducción a SQL | DataFrames, selección, filtros, cálculos, agrupaciones, ordenamiento y consultas SQL |
| `Clase 7` | Diagnóstico de calidad con Pandas | Reglas de calidad, faltantes, duplicados, tipos, rangos, fechas y decisiones de limpieza |
| `Clase 8` | Transformación y enriquecimiento | Variables derivadas, categorización de edades, descuentos, fechas y anticipación |
| `Clase_9` | Agrupaciones y análisis con `groupby` | Indicadores por periodo, programa y sede, denominadores, participación y cobertura |
| `Clase_10` | Integración de fuentes | Llaves, cardinalidad, tipos de unión, cobertura, conflictos y conservación de indicadores |

## Objetivos de aprendizaje

Al trabajar con este repositorio se practica cómo:

- usar Python como base para el análisis de datos;
- cargar e inspeccionar archivos CSV;
- reconocer tipos, estructura y calidad de un DataFrame;
- transformar columnas y crear variables analíticas;
- formular preguntas de negocio y responderlas con Pandas o SQL;
- distinguir filas, matrículas, estudiantes y entidades únicas;
- construir indicadores con denominadores explícitos;
- conservar faltantes y documentar las decisiones de limpieza;
- validar duplicados, llaves, fechas, rangos y valores contradictorios;
- integrar fuentes con uniones controladas y medir la cobertura del resultado.

## Requisito y forma de trabajo

El proyecto se trabaja desde **Google Colab conectado con Google Drive**. No es necesario instalar Python, Pandas, NumPy, Jupyter ni ningún otro programa en el equipo: Colab proporciona el entorno de ejecución y Drive permite guardar y organizar los notebooks y archivos del proyecto.

### Pasos para comenzar

1. Abre [Google Drive](https://drive.google.com/) e inicia sesión con tu cuenta de Google.
2. Guarda o sube en Drive este repositorio, o crea una carpeta para el proyecto con los notebooks y archivos CSV.
3. Abre [Google Colab](https://colab.research.google.com/) desde el navegador.
4. En Colab, abre el notebook (`.ipynb`) desde **Archivo > Abrir notebook > Google Drive**, o súbelo desde tu equipo.
5. Ejecuta la primera celda del notebook para montar Google Drive y autoriza el acceso cuando Colab lo solicite.
6. Verifica que la ruta indicada en el notebook coincida con la carpeta donde guardaste los archivos CSV.
7. Ejecuta las celdas en orden y guarda los cambios en Drive.

Los notebooks indican la carpeta esperada para cada clase y contienen las instrucciones necesarias para cargar los datos. Si reinicias el entorno de Colab, debes volver a montar Drive y ejecutar nuevamente las celdas de configuración. De esta forma, todo el trabajo se realiza en la nube y no necesitas hacer instalaciones locales.

## Cómo trabajar con los notebooks

1. Abre desde Drive el notebook de la clase que quieras estudiar.
2. Conecta Google Drive ejecutando la celda de montaje.
3. Mantén los archivos CSV en la carpeta indicada por el notebook.
4. Ejecuta las celdas en orden.
5. Completa únicamente las celdas marcadas con `COMPLETA AQUÍ`.
6. Revisa los resultados esperados y ejecuta los controles después de cada ejercicio.
7. Guarda el notebook con tus respuestas directamente en Drive.

Los notebooks usan señales para orientar el trabajo:

- **Recordemos:** concepto necesario para avanzar.
- **Ejemplo:** código resuelto.
- **Completa aquí:** actividad del estudiante.
- **Resultado esperado:** forma de comprobar el resultado.
- **Interpreta:** conexión entre el cálculo y la pregunta analítica.
- **Error frecuente:** dificultad habitual.
- **Extensión:** contenido opcional.

## Guía de archivos

### `Clase 3 y 4`

- `Laboratorio_1_Python_Fundamentos_ESUMER_v2.ipynb`: introducción a Python aplicada a un caso de e-commerce. Incluye variables, tipos, estructuras básicas, control de flujo, carga e inspección de un dataset y creación de reglas de negocio.

### `Clase 5`

- `Taller_Pandas_y_SQL_Ecommerce_ESUMER.ipynb`: taller de Pandas y consultas SQL sobre pedidos de una tienda virtual.
- `ventas_ecommerce.csv`: 96 pedidos, 30 clientes y 12 columnas con ciudad, canal, categoría, cantidades, precios, descuentos, estado y satisfacción.

El taller permite analizar categorías, ventas netas, pedidos de alto valor, ciudades y los cinco pedidos principales.

### `Clase 7`

- `Laboratorio_Pandas_Estudiantes.ipynb`: diagnóstico de calidad de una base ficticia de matrículas.
- `Matriculas_diagnostico.csv`: fuente inicial con matrículas, estudiantes, periodos, programas, sedes, fechas, estados, valores, descuentos y becas.

El laboratorio trabaja con reglas explícitas para identificadores, rangos de edad, fechas, valores, porcentajes, equivalencias de programas y campos desconocidos. Los faltantes se conservan como desconocidos cuando no existe evidencia para imputarlos.

### `Clase 8`

- `Laboratorio_Clase_8_Estudiantes.ipynb`: transformación y enriquecimiento de la base de matrículas.
- `Matriculas_diagnostico.csv`: copia de trabajo de la base de diagnóstico.

Se crean variables como valor de descuento, valor neto, rango de edad, días de anticipación y tipo de anticipación. El notebook conserva indicadores de revisión y permite comprobar que las transformaciones sean reproducibles.

### `Clase_9`

- `Laboratorio_Clase_9_Estudiantes.ipynb`: ejercicios de agrupación, agregación, participación y comparación por periodo.
- `Laboratorio_Clase_9_Resuelto.ipynb`: versión resuelta del laboratorio.
- `Matriculas_enriquecidas.csv`: base enriquecida proveniente del flujo de la clase 8.
- `Conflictos_llave_referencia.csv`: llaves con versiones contradictorias para revisión.
- `Copias_exactas_referencia.csv`: registros identificados como copias exactas.
- `Salidas/`: indicadores por programa y periodo, indicadores por sede y periodo, comparación de sedes y controles de integración.

La base de trabajo contiene 119 matrículas después de separar copias exactas y filas con conflictos de llave. Las cifras de matrícula no equivalen automáticamente a cantidad de estudiantes, facturación o recaudo.

### `Clase_10`

- `Laboratorio_Clase_10_Estudiantes.ipynb`: integración de fuentes de matrículas, estudiantes y programas.
- `Matriculas_2026-1.csv` y `Matriculas_2026-2.csv`: matrículas de dos periodos.
- `Maestro_estudiantes.csv`: maestro sintético de estudiantes.
- `Catalogo_programas.csv`: catálogo sintético de programas.
- `Salidas/`: resultados de integración, cobertura, conflictos, copias, llaves vacías y registros sin correspondencia.

El laboratorio verifica que la integración mantenga una fila por matrícula, evita emparejar llaves vacías, separa conflictos y deja visibles los registros sin estudiante o sin programa.

## Flujo recomendado

```text
Python y fundamentos
        |
        v
Pandas y SQL sobre e-commerce
        |
        v
Diagnóstico de calidad de matrículas
        |
        v
Transformación y enriquecimiento
        |
        v
Agrupaciones e indicadores
        |
        v
Integración de fuentes
```

La clase 9 puede utilizar `Matriculas_enriquecidas.csv` como resultado de la clase 8. La clase 10 trabaja con sus propias fuentes separadas por periodo y no requiere ejecutar los notebooks anteriores para comenzar. Las clases y materiales que aún no aparecen en este repositorio podrán agregarse posteriormente, a medida que avance el curso y los tenga disponibles.

## Criterios analíticos importantes

- Una fila de matrícula representa una matrícula, no necesariamente una persona única.
- Un estudiante puede tener varias matrículas en distintos periodos.
- `id_matricula` debe ser único; `id_estudiante` puede repetirse.
- Un valor neto calculado después del descuento no representa necesariamente facturación ni recaudo efectivo.
- Los valores faltantes no deben convertirse automáticamente en cero o en una categoría conocida.
- Los indicadores deben conservar su denominador y su universo de análisis.
- Las llaves vacías y las versiones contradictorias deben separarse para validación, no resolverse arbitrariamente.
- Antes y después de una unión deben comprobarse cardinalidad, unicidad, cobertura y cantidad de filas.

## Uso responsable

Este repositorio es material de formación. Si adaptas los notebooks a datos reales:

- trabaja sobre copias y conserva la fuente original;
- evita publicar datos personales o identificadores sensibles;
- documenta las reglas y decisiones de limpieza;
- valida los resultados con las áreas responsables;
- no reemplaces valores desconocidos sin una justificación verificable.

## Autoría y contexto académico

Este repositorio reúne material de apoyo y apuntes de trabajo del curso de Analítica y Visualización de Datos para la Toma de Decisiones de la universidad ESUMER / con apoyo de Estud-IA y La Alcaldia De Medellin. El docente identificado en los notebooks de las clases 8, 9 y 10 es **Johan Steev Muriel**.

## Resultados

En este repositorio se presentan análisis orientados a descubrir patrones, comparar variables y comunicar conclusiones mediante tablas, gráficos y dashboards.

## Autor

**Andrés Flórez**

Estudiante de Esumer Medellín.

- GitHub: [@Andresflorezdev](https://github.com/Andresflorezdev)

## Licencia

Este repositorio fue creado con fines académicos y educativos.
