# Reparto: cómo obtener la APK

Esta carpeta es un proyecto Flutter. GitHub lo compila gratis y te deja la APK lista para descargar en el celular.

## Pasos (desde una computadora)

1. Entra a github.com e inicia sesión (o crea una cuenta gratis).
2. Crea un repositorio nuevo, por ejemplo `reparto`. Puede ser privado.
3. En el repositorio vacío elige "uploading an existing file" y arrastra TODO el contenido de esta carpeta:
   `pubspec.yaml`, `lib`, `assets`, `LEEME.md` y la carpeta oculta `.github`.
   - Si no ves `.github` (en Mac y Linux las carpetas con punto están ocultas), crea el archivo a mano:
     "Add file" → "Create new file", escribe como nombre `.github/workflows/build-apk.yml`
     y pega el contenido del archivo `build-apk.yml`.
4. Confirma con "Commit changes". La compilación empieza sola.
   Puedes verla en la pestaña "Actions". Tarda unos 5 a 10 minutos.
5. Cuando termine, en la página principal del repositorio, columna derecha, abre "Releases".
   Ahí está `app-release.apk`.

## Instalar en el teléfono

1. Abre la página de Releases desde el navegador del celular y descarga `app-release.apk`.
2. Ábrelo. Android te pedirá permitir "instalar apps desconocidas" para el navegador. Acéptalo.
3. Instala. La app aparece como "Reparto".

## Notas

- Si la compilación falla, abre la ejecución en "Actions", copia el error y envíamelo.
- Los datos quedan guardados en el teléfono. Si desinstalas la app o borras sus datos, se pierden.
- Las tipografías se descargan de internet la primera vez. Sin conexión se usan las del sistema y todo funciona igual.
- La APK queda firmada con la clave de depuración. Sirve para uso personal.
