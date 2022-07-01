## ubuntu-comands
### Task Manager
```sh
gnome-system-monitor
```

### Удаление библиотек
```sh
dpkg --list
найти название библиотеки
```
```sh
sudo apt-get remove package-name
# удаление библиотеки
```
```sh
sudo apt-get purge package-name
# удаление персональных настроек
```
```sh
sudo apt-get autoremove
# удалить все устаревшие и неиспользуемые упакованные и оставшиеся зависимости
```

### Архивы  

```sh
tar -cvf archive.tar.gz /path/to/files
# архивировать файлы
```
```sh
tar -xvf archive.tar.gz
# чтобы распаковать архив 
```
### Изменить фоновое изображение в экране блокировки

```sh
wget github.com/thiggy01/change-gdm-background/raw/master/change-gdm-background
# загрузить скрипт
```

```sh
chmod +x change-gdm-background
# установить его как исполняемый файл
```
```sh
sudo ./change-gdm-background /path/to/image
# изменить фон
```
```diff
+ login image sucessfully changed
# успешно изменен
```
```sh
sudo ./change-gdm-background --restore
# восстановить исходную тему
```

### Скачать blob видео  
1. Найти в 'Network'-е 'file.m3u8' запрос на сервер 
2. Использовать url в 'Request URL': 'https://path/video.m3u8'
3. Запустить команду
```sh
ffmpeg -i 'https://path/video.m3u8' -c copy -bsf:a aac_adtstoasc 'video.mp4'
# video.mp4 видео на выходе
```

### Убрать точки в запущенных программах  
```sh
gsettings set org.gnome.shell.extensions.dash-to-dock custom-theme-running-dots 'false'
# true/false
```
### Конвертация файлов в pdf   
```sh
libreoffice --headless --invisible --convert-to pdf './path/file'
```
файлы в pdf
* конвертирует все файлы

### Слияние pdf документов  
```sh
pdfunite input1.pdf input2.pdf *.pdf output.pdf
```
### libinput-gesture  
https://github.com/bulletmark/libinput-gestures

### CoverflowAltTab  
https://github.com/dmo60/CoverflowAltTab

### Vitals(monitor pc)  
https://extensions.gnome.org/extension/1460/vitals/

### Control Fans mode for linux  
https://askubuntu.com/questions/1254364/how-to-control-fans-on-an-asus-laptop

### GREP regular expressions
https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux

### ОШИБКА У ВАС ЗАФИКСИРОВАНЫ СЛОМАННЫЕ ПАКЕТЫ
https://losst.ru/oshibka-u-vas-zafiksirovany-slomannye-pakety

### Установка драйвера видеокарты и cuda
1. https://forums.developer.nvidia.com/t/nvidia-smi-has-failed-because-it-couldnt-communicate-with-the-nvidia-driver-make-sure-that-the-latest-nvidia-driver-is-installed-and-running/197141/5
2. a) https://www.cyberciti.biz/faq/ubuntu-linux-install-nvidia-driver-latest-proprietary-driver/ <br>
   b) https://denishartl.com/installing-cuda-11-3-cudnn-tensorflow-2-4-jupyter-on-a-headless-ubuntu-20-04-server/
3. https://developer.nvidia.com/cuda-11.3.0-download-archive


### Manage RAM
```
htop
```
