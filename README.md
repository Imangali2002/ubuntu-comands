## ubuntu-comands
### Архивы<br>

```tar -cvf archive.tar.gz /path/to/files``` - архивировать файлы <br>
```tar -xvf archive.tar.gz``` - чтобы распаковать архив 

### Скачать blob видео<br>
ffmpeg -i 'https://path/video.m3u8' -c copy -bsf:a aac_adtstoasc 'video.mp4'
