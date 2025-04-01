# 🖥️ Guía de Configuración Rápida de Arch Linux con KDE Plasma

Esta es una guía rápida para instalar y configurar Arch Linux utilizando el comando `archinstall` y el entorno de escritorio KDE Plasma. También incluye la instalación de paquetes esenciales como **Firefox**, **Konsole** y **Neofetch**.

---

## 🚀 Instalación Inicial de Arch
Arranca desde la ISO de Arch Linux y ejecuta el siguiente comando para iniciar el instalador:

```bash
archinstall
```

---

## 🔑 Configuración de Usuario
Durante la instalación, establece la siguiente configuración:

- **Usuario:** `arch`
- **Contraseña:** `arch`

---

## 📦 Instalación de Paquetes Esenciales
Tras completar la instalación, inicia sesión en tu sistema y actualiza los paquetes:

```bash
sudo pacman -Syu
```

Luego, instala los paquetes esenciales:

```bash
sudo pacman -S firefox plasma-meta konsole neofetch
```

---

## 🖥️ Instalación de Xorg y KDE Plasma
Para configurar el entorno gráfico, instala el servidor Xorg:

```bash
sudo pacman -S xorg-server xorg-xinit
```

Instala el entorno de escritorio KDE Plasma:

```bash
sudo pacman -S plasma-desktop
```

---

## 🔳 Configuración del Gestor de Pantalla LightDM
Instala y habilita LightDM como gestor de inicio de sesión:

```bash
sudo pacman -S sddm
sudo systemctl enable sddm
sudo systemctl start sddm
```

---

## 🖼️ Selección del Entorno Gráfico
Al iniciar sesión, elige **Plasma (X11)** como entorno de escritorio.

---

## 🎨 Personalización y Comprobación
Para verificar la configuración y mostrar información del sistema en la terminal, usa:

```bash
neofetch
```

---

Ahora tienes Arch Linux instalado con KDE Plasma y listo para usar. 🚀

---
