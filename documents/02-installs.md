¿Cómo podemos añadir más dependencias? A través de Composer. 

Además de los paquetes «normales» de Composer, trabajaremos con dos tipos «especiales» de paquetes:
- Componentes Symfony: Paquetes que implementan las características principales y abstracciones de bajo nivel que la mayoría de las aplicaciones necesitan (enrutamiento, consola, cliente HTTP, mailer, caché, etc.);
- Bundles Symfony: Paquetes que añaden características de alto nivel o proporcionan integraciones con librerías de terceros (los bundles son, en su mayoría, aportados por la comunidad).

profiler es un alias para el paquete symfony/profiler-pack.
Los alias no son una característica propia de Composer, sino un concepto proporcionado por Symfony para hacer tu vida más fácil. Los alias son atajos para los paquetes populares de Composer.

¿Te has fijado en la opción --dev en el comando composer req? Como Symfony Profiler solo es útil durante la fase de desarrollo, queremos evitar que se instale en producción.

`symfony composer req profiler --dev`
- Symfony Profiler, una herramienta que te ayudará a ahorrar tiempo a la hora de identificar la causa de un problema
---
`symfony composer req logger`
- Logs
---
`symfony composer req debug --dev`
- Herramientas de depuración
---
`symfony composer req maker --dev`
- Maker bundle te ayuda a generar muchas clases diferentes
`symfony console list make`, para ver los comandos disponibles.
---
`symfony composer req annotations`
- Cuando llega una petición, alguna configuración necesita decirle a Symfony que la ruta de la petición debe ser gestionada por un controlador específico (una clase PHP). Cuando se utilizan formatos de configuración YAML, XML o PHP, hay dos archivos implicados (el archivo de configuración y el archivo PHP del controlador). Si se utilizan anotaciones, la configuración se realiza directamente en la clase de controlador.
