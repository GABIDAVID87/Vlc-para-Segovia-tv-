# Compilar VLC Android TV con GitHub Actions

1. Crea un repositorio vacío en GitHub.
2. Sube el **contenido de este proyecto** a la raíz del repositorio.
3. Abre **Actions** y selecciona **Build VLC Android TV**.
4. Pulsa **Run workflow**. También se ejecutará automáticamente al hacer push a `main` o `master`.
5. Cuando termine, abre la ejecución y descarga el artefacto **VLC-Android-TV-debug**.

El workflow instala Java 17, Android SDK 36, Build Tools 36.0.0, NDK 21.4.7075529 y Gradle 9.3.1.

La compilación es `debug`, por lo que no requiere una clave privada de firma.

Este paquete está preparado para Android TV/Leanback. Las variantes normales de la aplicación usan los artefactos LibVLC publicados por VideoLAN; el código fuente nativo de LibVLC no está incluido en este ZIP.
