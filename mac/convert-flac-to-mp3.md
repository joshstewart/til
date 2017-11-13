find . -name "*.flac" -exec ffmpeg -i {} -ab 192k -map_metadata 0 -id3v2_version 3 {}.mp3 \;
#find . -name "*.flac" -exec bash -c 'ffmpeg -i "{}" -y -acodec libmp3lame -ab 192k "${0/.flac}.mp3"' {} \;
