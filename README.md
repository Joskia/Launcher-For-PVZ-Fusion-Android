<div align="center">

# ⚡ FusionCore

**Runtime IL2CPP para modding en Android**

[![Platform](https://img.shields.io/badge/platform-Android-3DDC84?logo=android&logoColor=white)](#)
[![Arch](https://img.shields.io/badge/arch-arm64--v8a-blue)](#)
[![Runtime](https://img.shields.io/badge/runtime-BepInEx%20IL2CPP-orange)](#)
[![.NET](https://img.shields.io/badge/.NET-CoreCLR-512BD4?logo=dotnet&logoColor=white)](#)
[![License](https://img.shields.io/badge/original-All--Of--Us--Mods-lightgrey)](https://github.com/All-Of-Us-Mods/FusionCore.git)

*[Español](#-español) · [English](#-english)*

</div>

---

## 🇪🇸 Español

> Launcher/loader para Android que instala un runtime de **BepInEx IL2CPP (.NET/CoreCLR)** dentro de juegos Unity compatibles, permitiendo cargar mods nativos (DLL de C#) sin modificar el APK original del juego.

| | |
|---|---|
| 📦 **Package** | `dev.allofus.fusioncore` |
| 📱 **Plataforma** | Android · `arm64-v8a` |

### ⚙️ Qué hace

Al parchear un juego, FusionCore inyecta y ejecuta un runtime CoreCLR + BepInEx dentro del proceso del juego (vía hooking nativo), permitiendo que los mods `.dll` colocados en `BepInEx/plugins/` se carguen igual que en un mod de PC, pero contra ensamblados IL2CPP.

### 🎮 Juegos detectados en el manifiesto

-  `com.LanPiaoPiao.PlantsVsZombiesES`
-  `com.LanPiaoPiao.PlantsVsZombiesRH`
- Soporte genérico para actividades Unity (`unity3d.player.UnityPlayerActivity`), Firebase Messaging y otras integraciones (Among Us / `innersloth.spacemafia`, `teamcuriosity.addons`).

### 🚀 Uso típico

Instalar FusionCore → seleccionar el juego a parchear desde el selector → colocar los mods (`.dll` de BepInEx IL2CPP) en la carpeta `BepInEx/plugins/` generada para ese juego → lanzar el juego desde FusionCore. El runtime se inyecta automáticamente y carga los mods presentes.

> 💡 **Nota:** FusionCore es el **loader/runtime**, no un mod en sí — mods como `PCZFusionMod (OnePrime)` se ejecutan *sobre* FusionCore una vez instalado.

### 🛠️ Solución de problemas

Si al lanzar el juego aparece un error de Unity, ve a **Ajustes** y deshabilita la opción **"stripped libunity"**.

### 🙌 Créditos

- 🔗 Código original: [All-Of-Us-Mods/FusionCore](https://github.com/All-Of-Us-Mods/FusionCore.git)
- ✨ Versión modificada: **Joskia** (solo se mejoró la estética del launcher)

---

## 🇬🇧 English

> Android launcher/loader that installs a **BepInEx IL2CPP (.NET/CoreCLR)** runtime inside compatible Unity games, allowing native mods (C# DLLs) to be loaded without modifying the game's original APK.

| | |
|---|---|
| 📦 **Package** | `dev.allofus.fusioncore` |
| 📱 **Platform** | Android · `arm64-v8a` |

### ⚙️ What it does

When patching a game, FusionCore injects and runs a CoreCLR + BepInEx runtime inside the game's process (via native hooking), allowing `.dll` mods placed in `BepInEx/plugins/` to load just like a PC mod, but against IL2CPP assemblies.

### 🎮 Games detected in the manifest

-  `com.LanPiaoPiao.PlantsVsZombiesES`
-  `com.LanPiaoPiao.PlantsVsZombiesRH`
- Generic support for Unity activities (`unity3d.player.UnityPlayerActivity`), Firebase Messaging, and other integrations (Among Us / `innersloth.spacemafia`, `teamcuriosity.addons`).

### 🚀 Typical usage

Install FusionCore → select the target game from the selector → place the mods (BepInEx IL2CPP `.dll` files) in the `BepInEx/plugins/` folder generated for that game → launch the game from FusionCore. The runtime is injected automatically and loads the present mods.

> 💡 **Note:** FusionCore is the **loader/runtime**, not a mod itself — mods like `PCZFusionMod (OnePrime)` run *on top of* FusionCore once installed.

### 🛠️ Troubleshooting

If a Unity error appears when launching the game, go to **Settings** and disable the **"stripped libunity"** option.

### 🙌 Credits

- 🔗 Original code: [All-Of-Us-Mods/FusionCore](https://github.com/All-Of-Us-Mods/FusionCore.git)
- ✨ Modified version: **Joskia** (only the launcher's aesthetics were improved)
