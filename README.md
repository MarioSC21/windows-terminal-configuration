## Instalación de Oh My Posh

1. Asegúrate de tener instalado el [Terminal de Windows](https://apps.microsoft.com/detail/9N0DX20HK701?hl=en-us&gl=US).

2. Asegúrate de tener instalado [PowerShell](https://apps.microsoft.com/detail/9MZ1SNWT0N5D?hl=en-us&gl=US).

3. Abre la terminal y configúrala para usar PowerShell como el shell predeterminado.

### Instalación de Oh My Posh

Puedes instalar Oh My Posh de dos maneras:

#### Usando `winget`:

```bash
winget install JanDeDobbeleer.OhMyPosh -s winget
```

O a través de `Microsoft Store`:

#### Instalación de Oh My Posh a través de Microsoft Store

Descarga Oh My Posh desde [Microsoft Store](https://apps.microsoft.com/detail/XP8K0HKJFRXGCK?hl=en-us&gl=US).

1. En la terminal, crea un archivo de configuración con el siguiente comando:

    ```powershell
    New-Item -Path $PROFILE -Type File -Force
    ```

2. Abre el archivo de configuración con Notepad:

    ```powershell
    notepad $PROFILE
    ```

   Esto abrirá el archivo; dentro de él, copia la configuración por defecto que se encuentra en el archivo `oh-my-posh init pwsh --config $envP.txt` del repositorio.

3. Instala las fuentes que se encuentran en la carpeta `fonts` del repositorio, las cuales son Meslo y Hack.

4. Para instalar los iconos en la terminal, utiliza el siguiente comando:

    ```powershell
    Install-Module -Name Terminal-Icons -Repository PSGallery
    ```

5. Finaliza la personalización de la terminal abriendo el archivo `settings.json`. Para hacer esto, haz clic en el ícono de la rueda dentada en la configuración de la terminal y selecciona "Abrir archivo JSON". Después, usa `Ctrl + A` para seleccionar todo, borra el contenido y copia el contenido del archivo `Terminal-Apariencia.json` que se encuentra en el repositorio.


