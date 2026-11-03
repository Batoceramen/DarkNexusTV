# DARK NEXUS TV — proyecto inicial

Launcher Android TV minimalista para Android 9 (API 28), sin root y sin dependencias externas.

## Funciones de esta primera base
- Se registra como HOME / launcher y como Leanback Launcher.
- Descubre aplicaciones que exponen `LEANBACK_LAUNCHER`.
- Navegación con control remoto (DPAD) mediante foco Android.
- Reloj y fecha en pantalla.
- Interfaz oscura de alto contraste, sin red, anuncios ni telemetría propia.

## Compilar
Requiere Android Studio o AndroidIDE, JDK 17 y Android SDK Platform 34. Abre esta carpeta como proyecto Gradle y ejecuta `:app:assembleDebug`. APK: `app/build/outputs/apk/debug/app-debug.apk`.

## Instalar con ADB
`adb install -r app/build/outputs/apk/debug/app-debug.apk`

Al pulsar HOME, Android debería ofrecer elegir DARK NEXUS TV como aplicación de inicio. Mantén el launcher original como alternativa hasta probar todos los botones.

## Limitaciones de esta versión inicial
No modifica ni desactiva launchers del fabricante. No implementa todavía edición de favoritos, categorías, panel de ajustes ni gestión de fondo. Es una base funcional para probar compatibilidad y navegación en el MiTV-AESP0.
