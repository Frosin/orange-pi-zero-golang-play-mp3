# orange-pi-zero-golang-play-mp3
how to play mp3 with golang on orange pi zero

0. Активируем звуковую карту на устройстве: sudo armbian-config -> System -> Hardware -> ставим звездочку на analog codec, сохраняем, ребутимся
1. Orange pi zero имеет архитектуру armv7l, для меньшего гемора будем билдить прямо на устройстве, для этой архитектуры нет версии go, 
но есть совместимая для armv6, скачиваем ее и ставим https://golang.org/dl/go1.16.2.linux-armv6l.tar.gz
2. На устройстве инсталлим либу для работы со звуком sudo apt-get install libasound2-dev
3. Берем пример для работы с mp3: https://github.com/hajimehoshi/go-mp3/blob/master/example/main.go, 
заливаем исходинки и mp3 файл на устройство
4. Не забыв подключить колонку, слышим звук из устройства, радуемся.
