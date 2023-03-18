### Save all your files in the same folder
### Then type cmd, and then the folder
(example: my flac files are in a flac_audios folder at my desktop)
> cd desktop\flac_audios

> for /r %i in (*.flac) do ffmpeg -i "%i" -ab 320k -map_metadata 0 -id3v2_version 3 "%~ni.mp3"
