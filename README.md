# Angular16-Localize-es-en
 
Ejemplo para crear un proyecto en Angular 16 con la Internalización Localize.


1º Instalar las Dependencias

    npm install

2º Para lanzar el proyecto en cada idioma:

Lanzar el proyecto en Español: 

	ng serve --configuration=es

Lanzar el proyecto en Inglés: 

	ng serve --configuration=en


Tenemos que tener en cuenta el archivo de configuración Angular.json

    "projects": {
        "Tu nombre de proyecto": {
          "projectType": "application",
          "i18n": {
            "sourceLocale": "en-US",
            "locales": {
              "es-ES": "src/locale/messages.es.xlf"
            }
          },


Y en la sección de "configurations": {

Añadimos los idiomas:

     "es": {
                  "localize": ["es-ES"]
                },
                "en": {
                  "localize": ["en-US"]
                }

## Cuales son las ventajas de usar Localize en Angular

@angular/localize es una biblioteca en Angular que facilita la internacionalización (i18n) de las aplicaciones. Su uso ofrece varias ventajas clave, especialmente para proyectos que buscan llegar a una audiencia global. Algunas de estas ventajas incluyen:

1. Soporte Integrado para Múltiples Idiomas

Facilita la Traducción: Localize simplifica el proceso de traducción de tu aplicación a múltiples idiomas.
Manejo de Plurales y Selecciones: Proporciona una forma sencilla de manejar diferencias en plurales y selecciones entre idiomas.

2. Consistencia y Claridad

Centralización de Textos Traducibles: Los textos para traducir se extraen y se manejan de manera centralizada, lo que facilita su gestión.
Separación de Código y Contenido: Localize permite mantener el contenido traducible separado del código, lo que mejora la claridad y la mantenibilidad del código.

3. Fácil Integración y Uso

Integración con Angular CLI: Funciona sin problemas con Angular CLI, lo que facilita la extracción y manejo de traducciones.
Uso de Atributos Estándar: Utiliza el atributo i18n estándar en las plantillas HTML, lo que hace que sea fácil de aprender y aplicar.

4. Automatización

Extracción Automática de Textos: Permite la extracción automática de textos traducibles del código fuente.
Flujo de Trabajo Automatizado: Puede integrarse en un flujo de trabajo automatizado para la gestión de traducciones.

5. Flexibilidad y Escalabilidad

Compatible con Herramientas de Traducción: Los archivos de traducción están en formatos estándar (como XLIFF), lo que los hace compatibles con muchas herramientas de traducción.

Escalable para Proyectos Grandes: Funciona bien para proyectos grandes y complejos.

6. Mejora de la Experiencia del Usuario

Localización Efectiva: Aumenta la relevancia y accesibilidad de la aplicación para usuarios de diferentes regiones lingüísticas.

Soporte para Direccionalidad de Texto: Soporta idiomas con direccionalidad de texto diferente, como idiomas que se leen de derecha a izquierda.

7. Cumplimiento y Accesibilidad

Cumple con Estándares Internacionales: Ayuda a cumplir con los requisitos de accesibilidad y estándares internacionales.
Adaptable a Normativas Locales: Facilita la adaptación de tu aplicación a las normativas y preferencias culturales locales.

## Cual son las ventajas frente a ngx translate

@angular/localize y ngx-translate son dos enfoques populares para la internacionalización en aplicaciones Angular, cada uno con sus propias ventajas. Entender las diferencias y beneficios de cada uno puede ayudarte a elegir la mejor opción para tu proyecto. Aquí te muestro las ventajas de @angular/localize frente a ngx-translate:

1. Integración Nativa con Angular

Desarrollado por el Equipo de Angular: @angular/localize es mantenido por el equipo de Angular, asegurando una integración y compatibilidad nativa con el ecosistema Angular.
Actualizaciones Consistentes: Como parte del paquete Angular, recibe actualizaciones y mejoras regulares junto con el framework.

2. Rendimiento

Compilación AOT (Ahead-of-Time): @angular/localize funciona bien con la compilación AOT de Angular, lo que puede mejorar el rendimiento al reducir el tiempo de carga inicial y el tamaño del paquete.

3. Soporte de Angular CLI

Extracción Automática de Textos: La integración con Angular CLI permite una fácil extracción de textos traducibles, simplificando el proceso de manejo de múltiples idiomas.

4. Manejo de Plurales y Selecciones

Soporte Avanzado para Plurales y Selecciones: Ofrece capacidades integradas para manejar diferentes reglas de pluralización y selección entre idiomas, lo cual puede ser crítico en algunos idiomas.

5. Flujo de Trabajo Estático

Traducciones en Tiempo de Compilación: Las traducciones se aplican en tiempo de compilación, lo que puede resultar en un mejor rendimiento y una menor complejidad en tiempo de ejecución.

6. Facilidad de Uso y Mantenimiento

Menor Complejidad en el Código: Como las traducciones se manejan en tiempo de compilación, no hay necesidad de lógica adicional en el código para manejar el cambio de idiomas.

7. Soporte para Direccionalidad de Texto

Mejor Soporte para RTL (Right-to-Left): @angular/localize puede ofrecer un mejor soporte para idiomas que se leen de derecha a izquierda.

**Consideraciones al Elegir @angular/localize sobre ngx-translate:
**

Curva de Aprendizaje: @angular/localize puede tener una curva de aprendizaje más pronunciada, especialmente si no estás familiarizado con la internacionalización en Angular.

Flexibilidad: ngx-translate puede ser más flexible en escenarios donde las traducciones necesitan cargarse dinámicamente o ser modificadas en tiempo de ejecución.
Comunidad y Soporte: ngx-translate tiene una gran comunidad y una amplia base de usuarios, lo que puede ser útil para la resolución de problemas específicos y ejemplos de uso.

Cada herramienta tiene sus fortalezas y puede ser la mejor opción en diferentes contextos. La elección entre @angular/localize y ngx-translate dependerá de las necesidades específicas de tu proyecto, como los requisitos de rendimiento, la complejidad de las traducciones, y cómo planeas manejar el proceso de internacionalización.


