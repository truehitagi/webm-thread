**Анимублядский WebM-тред**
для приличных анимублядей и прочих аутистов.
Безграмотное быдло с дубляжом, войсовером, порнографией и котиками, советы мерзких мокрописечников, вниманиебляди всех видов и прочее непотребство отправляется в порнотред >>ссылка.

Для поиска сoуса видео сохраняем кадр (правый клик по видео) и ищем его на http://images.google.com.

Для воспроизведения **WebM с 10-битным цветом** нужно установить плагин vlc (http://nightlies.videolan.org/ ) и отключить встроенный в браузер плеер (media.webm.enabled=false в firefox).

**О кодировании WebM**
Доступные кодеки — VP8 и VP9 для видео, Vorbis и Opus для звука, **максимальный размер файла — 20480КБ** всех файлов в посте — 20480КБ (40960КБ с пасскодом).
**Делать WebM** можно научиться в вики треда: https://github.com/pituz/webm-thread/wiki/
Там находится подробная информация о выборе и настройке кодеков на примерах использования консольных утилит ffmpeg, vpxenc и mkvmerge.

**Неочевидные моменты**
— libvorbis при указании битрейта (-b:a) работает в режиме CBR (постоянный битрейт), и это портит качество звука; для режима VBR вместо битрейта надо указывать качество (-q:a); параметр -vbr on работает только для Opus'а;
— в webm'ки не нужно включать софтсаб в формате webvtt (FFmpeg это делает по умолчанию при наличии сабов в контейнере, отключается параметром **-sn**): во-первых, это бесполезно (для его отображения на странице должен быть специальный код), а во-вторых, от этого ролики не воспроизводятся в firefox.

**Программы и их документация**
http://webmproject.org http://ffmpeg.org http://mpv.io http://www.bunkus.org/videotools/mkvtoolnix/

**Фронтенды к ffmpeg для кодирования вебмок**
CLI, бидон: https://pypi.python.org/pypi/webm
CLI, zsh: https://github.com/pituz/webm-thread/tree/master/tools
CLI, дотнет: https://github.com/CherryPerry/ffmpeg-vp9-wrap
GUI, дотнет: https://gitgud.io/nixx/WebMConverter

**Оп-паста**: https://raw.githubusercontent.com/truehitagi/webm-thread/master/README.md
