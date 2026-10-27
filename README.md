# CamaraApp

App Android (Java) que abre la cámara del dispositivo con un Intent `ACTION_IMAGE_CAPTURE` y muestra la foto tomada en un `ImageView`.

## Estructura

- `app/src/main/AndroidManifest.xml`: permiso de cámara y sección `<queries>` necesaria en Android 11+ (API 30+).
- `app/src/main/res/layout/activity_main.xml`: `RelativeLayout` con un `ImageView` y el botón "Abrir Cámara".
- `app/src/main/java/com/example/camaraapp/MainActivity.java`: **Opción B** (recomendada), usa `ActivityResultLauncher` / `ActivityResultContracts`.
- `docs/MainActivity_OpcionA.java`: **Opción A**, estructura original con `startActivityForResult` / `onActivityResult`, corregida para evitar cierres inesperados.

## Cómo ejecutar

1. Abrir la carpeta en Android Studio.
2. Sincronizar Gradle.
3. Ejecutar en un dispositivo o emulador con cámara.
