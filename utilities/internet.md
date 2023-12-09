## wget - download a complete directory
 wget --no-parent -r http://WEBSITE.com/DIRECTORY

## Download only mp3
wget -c -A '*.mp3' -r -l 1 -nd http://example.org/musics/