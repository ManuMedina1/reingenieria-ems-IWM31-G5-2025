# Reingeniería y Migración del Sistema Legado de Gestión Académica

**<u>Introducción</u>**

Este repositorio contiene la documentación, código y artefactos resultantes del proceso de **reingeniería** y **migración** de un sistema legado crítico desarrollado en **Java** para la gestión de la información académica de asignaturas. El objetivo es transformar un sistema tradicional de escritorio en una aplicación moderna, escalable y orientada a la entrega incremental, que responda a las demandas actuales de accesibilidad y funcionalidad.

## **Antecedentes**

En el pasado, la ETSISI desarrolló una aplicación en Java para gestionar gran parte de la información académica. Con el tiempo, el sistema se volvió obsoleto debido a diversas limitaciones:

- **Accesibilidad Limitada:** La aplicación solo era compatible con sistemas de escritorio, impidiendo su uso en dispositivos móviles.
- **Mantenimiento Inadecuado:** La falta de soporte y actualización causó que la aplicación presentara fallos y restricciones en su funcionamiento.
- **Documentación Escasa:** Solo se conserva un **Javadoc** que obliga a realizar un proceso de **ingeniería inversa** para recuperar los modelos y especificaciones del sistema.

## **Objetivos del Proyecto**

El proyecto se estructura en tres fases:

1. **_Entender el Sistema Legado_**
   - Recuperar la documentación existente mediante ingeniería inversa.
   - Obtener el modelo lógico y el diagrama E/R de la base de datos.
   - Analizar la arquitectura actual: organización de paquetes y comunicación entre componentes.
   - Elaborar un diagrama de clases simplificado.
   - Especificar los requisitos funcionales en formato tradicional o ágil.

2. **_Re-especificación y Rediseño_**
   - Actualizar los requisitos funcionales basados en el análisis y transcripción de entrevistas.
   - Diseñar un nuevo modelo de base de datos ajustado a los nuevos requerimientos.
   - Rediseñar la arquitectura de la aplicación y elaborar un diagrama de clases de la capa de negocio.

3. **_Plan de Migración_**
   - **Definir y justificar** la estrategia de migración (por ejemplo, *Chicken Little* u otra alternativa).
   - Elaborar un plan detallado del proceso de migración, dividiendo la migración en fases:
     - **Migración de Datos:** Uso de scripts, componentes ETL o gateways.
     - **Migración del Software:** Estrategias de integración continua, control de versiones, despliegue incremental y mockups de la aplicación.
   - Permitir la validación progresiva y obteniendo _feedback_ de los usuarios durante el proceso.

## **Estructura del Repositorio**

- **/docs**  
  Documentación general del proyecto: enunciados, especificaciones de requisitos, casos de uso y transcripciones.

- **/design**  
  Modelos y diagramas:
  - Diagrama E/R y modelo lógico de la base de datos.
  - Diagramas de clases y arquitectura del sistema legado.
  - Propuestas de rediseño de base de datos y la arquitectura de la aplicación.

- **/migration**  
  Estrategia y plan de acción:
  - Descripción del proceso de migración de datos y software.
  - Scripts y pseudocódigo relacionados con componentes adicionales (gateways, ETLs).

- **/src**  
  Código fuente de la nueva aplicación o prototipos.

- **/legacy**  
  Artefactos y recursos del sistema antiguo, cuando sean necesarios para referencia.

## **Metodología y Herramientas**

Este proyecto se desarrollará de manera **iterativa** e **incremental**, permitiendo la entrega continua de nuevas funcionalidades. Los principales enfoques y herramientas son:

- **Ingeniería Inversa:**  
  Utilización del Javadoc y análisis del código legado para recuperar la documentación y entender la arquitectura original.

- **Re-especificación de Requisitos:**  
  Actualización de las especificaciones basadas en el análisis de reuniones y entrevistas, asegurando que los requerimientos sean claros y completos.

- **Rediseño de la Aplicación:**  
  Propuesta de una nueva arquitectura (por ejemplo, basada en microservicios o en una estructura modular en capas) que permita facilitar la migración y escalabilidad.

- **Plan de Migración Detallado:**  
  Definición clara de las fases y estrategias de migración, considerando:
  - Migración de datos mediante scripts y herramientas ETL.
  - Integración continua y despliegue incremental para minimizar la interrupción del servicio.
  - Estrategia de pruebas y validación con **feedback** directo de los usuarios.

---

**<u>Nota:</u>**  
El propósito de este proyecto es garantizar la continuidad del servicio durante la transición del sistema legado al nuevo entorno tecnológico, asegurando la operatividad crítica del sistema académico.

---

*Proyecto realizado como parte de la práctica "Reingeniería y Migración de un Sistema Legado/Crítico" para la ETSISI.*
