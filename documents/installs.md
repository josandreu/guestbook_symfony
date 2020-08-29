¿Cómo podemos añadir más dependencias? A través de Composer. 

Además de los paquetes «normales» de Composer, trabajaremos con dos tipos «especiales» de paquetes:
- Componentes Symfony: Paquetes que implementan las características principales y abstracciones de bajo nivel que la mayoría de las aplicaciones necesitan (enrutamiento, consola, cliente HTTP, mailer, caché, etc.);
- Bundles Symfony: Paquetes que añaden características de alto nivel o proporcionan integraciones con librerías de terceros (los bundles son, en su mayoría, aportados por la comunidad).

symfony composer req profiler --dev

symfony composer req logger

symfony composer req debug --dev

