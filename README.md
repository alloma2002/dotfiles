# 💻 My Personal Dotfiles | Titix Edition
**Hacking Station & Workflow Optimization**

Este repositorio contiene mis archivos de configuración personal para un entorno basado en **bspwm**. Está diseñado para la máxima eficiencia en auditorías, optimizando el consumo de recursos y el uso de atajos de teclado.

## 🛠️ Stack Tecnológico

### 🖥️ Entorno Gráfico (UI/UX)
- **WM**: [bspwm](https://github.com/baskerville/bspwm) + [sxhkd](https://github.com/baskerville/sxhkd) (Gestión de ventanas y atajos).
- **Terminal**: [Kitty](https://sw.kovidgoyal.net/kitty/) (Renderizado por GPU).
- **Compositor**: [Picom](https://github.com/yshui/picom) (Transparencias).
- **Lanzador**: [Rofi](https://github.com/davatorium/rofi).
- **Wallpaper**: [Feh](https://feh.finalrew.jp/).

### 🐚 Herramientas de Consola & Edición
- **Editor**: [Neovim](https://neovim.io/) + [NvChad](https://nvchad.com/).
- **Explorador**: [Ranger](https://github.com/ranger/ranger).
- **Productividad**: `fzf`, `batcat`, `lsd`, `locate`.
- **Fuentes**: [Hack Nerd Fonts](https://www.nerdfonts.com/).

## 📂 Estructura del Repositorio
Siguiendo el estándar de Linux, las configuraciones se organizan bajo el directorio `.config/`:
- `.config/bspwm/`: Configuración del gestor de ventanas (`bspwmrc`).
- `.config/kitty/`: Personalización de la terminal (`kitty.conf`).
- `.config/sxhkd/`: Mapeo de atajos de teclado (`sxhkdrc`).

## 🚀 Cómo aplicar las configuraciones
> [!CAUTION]
> Haz un backup de tus carpetas originales en `~/.config/` antes de proceder.

```bash
# 1. Clona el repositorio
git clone [https://github.com/alloma2002/dotfiles.git](https://github.com/alloma2002/dotfiles.git) ~/dotfiles_temp

# 2. Copia las configuraciones a tu carpeta .config
cp -rv ~/dotfiles_temp/.config/* ~/.config/

# 3. Recarga bspwm y sxhkd
bspc wm -r
