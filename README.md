# RIO10K para Windows

Aplicación local portátil para dirigir tu torneo de Texas Hold’em. Incluye el runtime oficial de Node.js; no necesitas instalar Node, npm ni una clave API.

## Descargar

1. Abre [RIO10K-Windows.zip](./RIO10K-Windows.zip).
2. Pulsa el icono **Download raw file** (flecha hacia abajo) de GitHub. Si el repositorio es privado, inicia sesión con la cuenta que tiene acceso.
3. En Windows, haz clic derecho sobre el ZIP y selecciona **Extraer todo**. No ejecutes el iniciador desde dentro del ZIP.
4. Abre la carpeta `RIO10K` y haz doble clic en **ABRIR-RIO10K.bat**.
5. Entra con el PIN inicial **1010** y cámbialo en Configuración.

**[Enlace directo al ZIP](https://github.com/edudu7447/gpt-edu1/raw/refs/heads/descarga-rio10k-windows/RIO10K-Windows.zip)**

Mantén abierta la ventana del iniciador mientras diriges el torneo; puedes minimizarla. Con Chrome o Edge, la app se abre como una ventana independiente. Si el navegador no se abre automáticamente, abre `http://127.0.0.1:4178` en el equipo donde ejecutaste el iniciador.

## Datos y respaldos

El torneo funciona sin internet y se guarda en el mismo navegador/perfil del equipo. Exporta respaldos JSON desde Configuración. No uses modo incógnito ni borres los datos del sitio si quieres conservarlo. Para pasar el torneo a otro equipo, exporta e importa el JSON.

Incluye jugadores ficticios para probar. En Configuración → Nuevo torneo puedes iniciar tu evento con la sala vacía.

## Compatibilidad y verificación

Paquete para Windows de 64 bits (Intel/AMD), con una versión de Windows compatible con Node.js 24 y un navegador moderno. La ejecución completa fue validada en Linux; el runtime Windows se verificó con el SHA-256 oficial de Node.js, pero no se ejecutó en Windows durante la preparación.

Archivo de aproximadamente 34 MiB. Puedes verificarlo en PowerShell:

```powershell
Get-FileHash .\RIO10K-Windows.zip -Algorithm SHA256
```

SHA-256:

```text
a404dc15779ac71b45043d2053fa8638a3c26f40b3a4309cab424b7e646e8be6
```

Esta rama contiene únicamente el paquete descargable y estas instrucciones. No cambia la aplicación ni los archivos de trabajo del proyecto.
