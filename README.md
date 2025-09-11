````
# ⚡ Первоначальная настройка и установка пакетов  

После установки Arch Linux и Hyprland пришло время настроить систему под себя 🚀  
````
---

## 🛠️ 1. Установка базовых пакетов  

Устанавливаем нужный софт и шрифты:  

```
yay git fish wofi hyprpaper hyprlock kitty thynar hyprshot dunst waybar ark 7z google-chrome telegram-desktop
````

````
sudo pacman -S pkgfile powerline-fonts inetutils nwg-look papirus-icon-theme fastfetch meson
````

````
sudo pacman -S noto-fonts-emoji noto-fonts noto-fonts-extra
````

````
sudo pacman -S ttf-font-awesome otf-font-awesome ttf-jetbrains-mono ttf-dejavu
````

---

## 📂 2. Клонирование дополнительных конфигов

````
git clone https://github.com/Aptivace/hyprland-config
````
````
git clone https://github.com/vinceliuice/Graphite-gtk-theme
````
````
git clone https://github.com/ArtsyMacaw/wlogout.git
```


````
## 🎨 3. Применение конфигов

### 🖥️ Kitty

````
cd hyprland-config/kitty
````
````
cp kitty.conf ~/.config/kitty
````

Закройте все активные терминалы (**Win+Q**).

---

### ⚙️ Hyprland + Waybar + Wofi

````
cd hyprland-config/
````
````
cp -r waybar ~/.config
````
````
cp -r wofi ~/.config
````
````
cd
```

---
````
### 🎭 GTK-тема

````
cd Graphite-gtk-theme
````
````
./install.sh
```
````
Теперь:

1. Нажмите **Win+R** и откройте **Gtk-settings**.
2. Примените тему: `Graphite-Dark` или `Graphite-Light`.
3. Выберите иконки: `Papirus-Dark` или `Papirus-Light`.

---

### 🔒 Wlogout

````
cd ~/wlogout
````
````
meson build
````
````
ninja -C build
````
````
sudo ninja -C build install
````
````
cd
```

---
````
### 🐟 Fish shell

````
chsh
````
````
/bin/fish
```

---
````
## 🔄 Завершающий шаг

Осталось только перезагрузить компьютер:

````
reboot
````

или используйте **Win+O**.

---

# 🎉 Поздравляю!

Настройка завершена. Теперь у вас готовая и красивая рабочая среда на **Arch Linux + Hyprland** 🌿

```
```
