## ubuntu-comands
### Удаление библиотек
```sh
dpkg --list
# найти название библиотеки
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

### Архивы<br>

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

### Скачать blob видео<br>
1. Найти в 'Network'-е 'file.m3u8' запрос на сервер 
2. Использовать url в 'Request URL': 'https://path/video.m3u8'
3. Запустить команду
```sh
ffmpeg -i 'https://path/video.m3u8' -c copy -bsf:a aac_adtstoasc 'video.mp4'
# video.mp4 видео на выходе
```

### Убрать точки в запущенных программах<br>
```sh
gsettings set org.gnome.shell.extensions.dash-to-dock custom-theme-running-dots 'false'
# true/false
```
### Конвертация файлов в pdf<br>
```sh
libreoffice --headless --invisible --convert-to pdf './path/file'
# файлы в pdf
# * конвертирует все файлы
```

### Слияние pdf документов<br>
```sh
pdfunite input1.pdf input2.pdf *.pdf output.pdf
```
