## ubuntu-comands
### Архивы<br>

```tar -cvf archive.tar.gz /path/to/files``` - архивировать файлы <br>
```tar -xvf archive.tar.gz``` - чтобы распаковать архив 

### Скачать blob видео<br>
1. Найти в 'Network'-е 'file.m3u8' запрос на сервер 
2. Использовать url в 'Request URL': 'https://path/video.m3u8'
3. Запустить команду ```ffmpeg -i 'https://path/video.m3u8' -c copy -bsf:a aac_adtstoasc 'video.mp4'```
