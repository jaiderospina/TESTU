# Framework de Zachman: Ontología de Arquitectura Empresarial

Este repositorio contiene una guía técnica sobre el **Framework de Zachman**, una estructura lógica diseñada para clasificar y organizar las representaciones descriptivas de una organización o sistema de información.

## 📌 Introducción

![]()

Propuesto por John Zachman en 1987, este esquema no es una metodología ni un proceso de diseño, sino una **ontología**. Su función principal es asegurar que todos los componentes críticos de una arquitectura sean considerados desde múltiples perspectivas, evitando vacíos de información.

---

## 🛠 Estructura de la Matriz (6x6)

La potencia del framework reside en su matriz, que cruza **Interrogantes** fundamentales con **Perspectivas** de abstracción.

### 1. Las Columnas (Interrogantes)
Responden al "qué", "cómo", "dónde", "quién", "cuándo" y "por qué" de la empresa.

| Interrogante | Foco | Descripción |
| :--- | :--- | :--- |
| **Qué** | **Datos** | Entidades, objetos e información relevante para el negocio. |
| **Cómo** | **Funciones** | Procesos, flujos de trabajo y transformaciones de entrada/salida. |
| **Dónde** | **Red** | Distribución geográfica, nodos y conexiones de infraestructura. |
| **Quién** | **Personas** | Actores, roles, responsabilidades y estructura organizacional. |
| **Cuándo** | **Tiempo** | Ciclo de vida, eventos, cronogramas y dependencias temporales. |
| **Por qué** | **Motivación** | Metas, estrategias, reglas de negocio y objetivos tácticos. |

### 2. Las Filas (Perspectivas)
Representan los niveles de abstracción desde la estrategia hasta la ejecución.

1. **Contextual (Planificador):** Visión de alto nivel y definición del alcance.
2. **Conceptual (Dueño):** El modelo del negocio y sus reglas operativas.
3. **Lógica (Diseñador):** Traducción a requerimientos de sistema (tecnológicamente agnóstico).
4. **Física (Constructor):** Arquitectura técnica y selección de herramientas/plataformas.
5. **Detallada (Subcontratista):** Especificaciones técnicas de componentes y módulos.
6. **El Producto (Usuario):** El sistema final en el entorno de producción.

---

## ⚖️ Reglas Fundamentales

Para garantizar la integridad del modelo, se deben seguir estos principios:

* **Unicidad:** Cada celda es única; la información no debe duplicarse en otras celdas.
* **Igualdad:** Todas las columnas tienen la misma importancia para la arquitectura global.
* **Completitud:** La arquitectura solo está "terminada" cuando las 36 celdas están definidas y alineadas entre sí.

---

## 🚀 Aplicación Práctica

A diferencia de frameworks basados en procesos (como TOGAF), Zachman se enfoca en la **clasificación y gobernanza**:

* **Identificación de Gaps:** Visualiza rápidamente qué áreas de la organización carecen de documentación.
* **Alineación Estratégica:** Permite que los roles directivos y técnicos hablen un lenguaje común.
* **Análisis de Impacto:** Ayuda a predecir cómo un cambio en la estrategia (Fila 1) afectará a los nodos de red o bases de datos (Fila 4).

---

> [!TIP]
> Este framework es especialmente útil en entornos de alta complejidad, como la **ciberdefensa** o la **gobernanza de identidad digital**, donde la trazabilidad entre el objetivo y la implementación es crítica.

---




Analizar el riesgo cibernético no es solo adivinar qué podría salir mal; es un proceso estructurado para entender qué activos tenemos, qué tan vulnerables son y qué tan fuerte nos golpearía un ataque.

Aquí tienes una definición de las técnicas más utilizadas, clasificadas por su enfoque:

---

### 1. Técnicas Cualitativas
Estas técnicas se basan en el juicio de expertos y escalas descriptivas (como "Bajo", "Medio", "Alto"). Son ideales cuando no se dispone de datos numéricos precisos.

* **Matriz de Riesgos (Heat Map):** Es la técnica más común. Cruza la **Probabilidad** de que ocurra un evento con el **Impacto** que causaría.
* **Análisis Histórico:** Se revisan incidentes pasados dentro de la organización o en el sector industrial para predecir escenarios futuros.
* **Entrevistas y Delphi:** Consultas a expertos para obtener un consenso sobre cuáles son las amenazas más críticas.



---

### 2. Técnicas Cuantitativas
Buscan asignar un valor numérico (generalmente monetario) al riesgo. Son más complejas pero permiten una mejor toma de decisiones financiera.

* **ALE (Annual Loss Expectancy):** Calcula cuánto dinero se espera perder al año por un riesgo específico. La fórmula es:
    $$ALE = SLE \times ARO$$
    Donde $SLE$ es la pérdida por un solo evento y $ARO$ es la tasa de ocurrencia anual.
* **Simulación de Montecarlo:** Un método algorítmico que utiliza iteraciones aleatorias para predecir la probabilidad de diferentes resultados en situaciones inciertas.
* **Análisis del Árbol de Fallos (FTA):** Una técnica deductiva que comienza con un evento no deseado y analiza todas las posibles formas en que pudo ocurrir.

---

### 3. Técnicas Semicuantitativas
Utilizan escalas numéricas (ej. del 1 al 10) para dar una sensación de precisión sin llegar a la complejidad de un análisis financiero total. Un ejemplo clásico es el **CVSS (Common Vulnerability Scoring System)**, que califica las vulnerabilidades del software.

---

### 4. Metodologías y Marcos de Trabajo (Frameworks)
Más que técnicas aisladas, son sistemas completos para gestionar el riesgo:

| Metodología | Enfoque Principal |
| :--- | :--- |
| **NIST 800-30** | Estándar federal de EE. UU. muy detallado para sistemas de TI. |
| **ISO/IEC 27005** | Enfoque internacional basado en el ciclo de mejora continua. |
| **MAGERIT** | Metodología española muy robusta, ideal para la administración pública y grandes empresas. |
| **FAIR (Factor Analysis of Information Risk)** | Un modelo específico para cuantificar el riesgo en términos económicos. |

---

### Resumen de Diferencias

> **Nota:** La elección de la técnica depende de la madurez de la empresa. Las startups suelen empezar con matrices **cualitativas**, mientras que las entidades bancarias suelen utilizar modelos **cuantitativos** complejos.

¿Estás buscando implementar alguna de estas técnicas en un entorno específico o necesitas ayuda para calcular un riesgo en particular?
