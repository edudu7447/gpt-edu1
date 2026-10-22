# RIO10K para Windows

Aplicación local portátil para dirigir tu torneo de Texas Hold’em. Incluye el runtime oficial de Node.js; no necesitas instalar Node, npm ni una clave API.

## Edición negro, dorado y mármol

La aplicación usa los colores del afiche proporcionado y una adaptación de su logo central con fondo transparente. El logo grande se muestra como marca de agua detrás del reloj y también aparece en acceso, TV, iconos y reportes. Para una reproducción exacta se puede reemplazar por el PNG transparente o SVG original del organizador.

![Vista previa del panel RIO10K](./Vista-previa.png)

## Descargar

1. Abre [RIO10K-Windows.zip](./RIO10K-Windows.zip).
2. Pulsa el icono **Download raw file** (flecha hacia abajo) de GitHub. Si el repositorio es privado, inicia sesión con la cuenta que tiene acceso.
3. En Windows, haz clic derecho sobre el ZIP y selecciona **Extraer todo**. No ejecutes el iniciador desde dentro del ZIP.
4. Abre la carpeta `RIO10K` y haz doble clic en **ABRIR-RIO10K.bat**.
5. Entra con el PIN inicial **1010** y cámbialo en Configuración.

**[Enlace directo al ZIP](https://github.com/edudu7447/gpt-edu1/raw/refs/heads/descarga-rio10k-windows/RIO10K-Windows.zip)**

Mantén abierta la ventana del iniciador mientras diriges el torneo; puedes minimizarla. Con Chrome o Edge, la app se abre como una ventana independiente. Si el navegador no se abre automáticamente, abre `http://127.0.0.1:4178` en el equipo donde ejecutaste el iniciador.

## Actualizar una instalación anterior

1. Exporta primero un respaldo JSON desde Configuración.
2. Cierra las ventanas RIO10K/TV y el iniciador anterior.
3. Extrae el nuevo ZIP en otra carpeta y abre su ABRIR-RIO10K.bat.
4. Usa el mismo navegador/perfil; el origen sigue siendo http://127.0.0.1:4178, por lo que tus datos se conservan.
5. Si aparece el estilo anterior, espera unos segundos a que se guarde la actualización, cierra todas las ventanas RIO10K y vuelve a abrir el iniciador. **No borres los datos del sitio**.

## Datos y respaldos

El torneo funciona sin internet y se guarda en el mismo navegador/perfil del equipo. Exporta respaldos JSON desde Configuración. No uses modo incógnito ni borres los datos del sitio si quieres conservarlo. Para pasar el torneo a otro equipo, exporta e importa el JSON.

Incluye jugadores ficticios para probar. En Configuración → Nuevo torneo puedes iniciar tu evento con la sala vacía.

## Compatibilidad y verificación

Paquete para Windows de 64 bits (Intel/AMD), con una versión de Windows compatible con Node.js 24 y un navegador moderno. La ejecución completa fue validada en Linux; el runtime Windows se verificó con el SHA-256 oficial de Node.js, pero no se ejecutó en Windows durante la preparación.

Archivo de aproximadamente 35 MiB. Puedes verificarlo en PowerShell:

```powershell
Get-FileHash .\RIO10K-Windows.zip -Algorithm SHA256
```

SHA-256:

```text
f317be450d3aeb2dcd59547861315c3a5039db6a3870723e126ed6c073999500
```

Esta rama contiene únicamente el paquete descargable y estas instrucciones. No cambia la aplicación ni los archivos de trabajo del proyecto.
