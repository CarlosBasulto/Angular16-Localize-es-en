# Angular16-Localize-es-en
 

Ejemplo para crear un proyecto en Angular 16 con la Internalización Localize.

 Instalar las Dependencias

npm install


Lanzar el proyecto en Español: ng serve --configuration=es

Lanzar el proyecto en Inglés: ng serve --configuration=en


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