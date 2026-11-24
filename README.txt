MI TV - PROYECTO ANDROID PARA GITHUB ACTIONS

SUBIDA:
1. Descomprimí MI-TV-GitHub.zip.
2. Subí el CONTENIDO de la carpeta a la raíz de un repositorio GitHub.
3. En la raíz deben verse app/, .github/, build.gradle, settings.gradle y gradle.properties.
4. Abrí Actions y ejecutá "Build MI TV APK" con Run workflow.
5. Al terminar, descargá el artefacto MI-TV-debug.

CONFIGURACIÓN:
- Paquete: com.mitv.app
- Java: 17
- Backend previsto: https://teve.totalh.net/tvserver/api/
- Reproductor: Android Media3 / ExoPlayer.

INCLUYE:
- Carga de listas M3U/M3U8 desde URL.
- Lectura de nombre, grupo, logo y URL de cada canal.
- Acceso Xtream mediante get.php.
- Reproducción de streams compatibles con Media3 (HLS y MP4, entre otros soportados).
- Los enlaces YouTube se abren en una aplicación/navegador compatible.
- Panel ADMIN dentro de la aplicación, con contraseña creada en el primer acceso.

IMPORTANTE:
El panel de esta primera base administra fuentes de listas en el dispositivo. No modifica todavía canales,
usuarios ni datos MySQL. Para sincronizar el panel con el backend real necesito revisar los PHP actuales
de /tvserver y sus endpoints. No inventé rutas de API ni un sistema de autenticación de servidor.

Algunos streams TS pueden necesitar cabeceras, tokens o permisos del proveedor. No se incluyen listas
ni enlaces de canales. Usá únicamente fuentes que tengas autorización para reproducir.
