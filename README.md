# Первоначальная настройка и установка пакетов

## 1 Установка базовых пакетов
Для начало давайте установим все необходимые пакеты и зависимости к ним
````
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

## 2 Скопируем дополнительные конфиги
````
git clone https://github.com/Aptivace/hyprland-config
````
````
git clone https://github.com/vinceliuice/Graphite-gtk-theme
````
````
git clone https://github.com/ArtsyMacaw/wlogout.git
````

## 3 Начнем применять эти конфиги
````
cd hyprland-config/kitty
````
````
cp kitty.conf ~/.config/kitty
````
````
закрыть все активные терминалы "win+Q"
````
````
cd hypr
````
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
````
````
cd Graphite-gtk-theme
````
````
.install.sh
````
````
проверить нажатием win+R и открыть там Gtk-settings, применить тему Graphite-Dark\light и применить иконки papirus-Dark\light
````
````
cd
````
````
cd wlogout/
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
````
````
chsh
````
````
bin/fish
````
## Осталось только перезагрузить компьютер и конфиги готовы
````
reboot либо win+O
````
Наша настройка завершенна, поздравляю с установкой arch linux
