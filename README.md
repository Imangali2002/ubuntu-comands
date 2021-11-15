## ubuntu-comands
### Удаление библиотек<br>
```dpkg --list``` - найти название библиотеки<br>
```sudo apt-get remove package-name``` - удаление библиотеки<br>
```sudo apt-get purge package-name``` - удаление персональных настроек<br>
```sudo apt-get autoremove``` - удалить все устаревшие и неиспользуемые упакованные и оставшиеся зависимости

### Архивы<br>

```tar -cvf archive.tar.gz /path/to/files``` - архивировать файлы <br>
```tar -xvf archive.tar.gz``` - чтобы распаковать архив 

### Изменить фоновое изображение в экране блокировки<br>

```wget github.com/thiggy01/change-gdm-background/raw/master/change-gdm-background``` - загрузить скрипт<br>
```chmod +x change-gdm-background``` - установить его как исполняемый файл<br>
```sudo ./change-gdm-background /path/to/image```  - изменить фон<br>
login image sucessfully changed<br>
```sudo ./change-gdm-background --restore``` - восстановить исходную тему

### Скачать blob видео<br>
1. Найти в 'Network'-е 'file.m3u8' запрос на сервер 
2. Использовать url в 'Request URL': 'https://path/video.m3u8'
3. Запустить команду ```ffmpeg -i 'https://path/video.m3u8' -c copy -bsf:a aac_adtstoasc 'video.mp4'``  ```

### Убрать точки в запущенных программах<br>
```gsettings set org.gnome.shell.extensions.dash-to-dock custom-theme-running-dots 'false'``` 
