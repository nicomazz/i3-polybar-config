the script `ng_wallpaper.py` download the national geographic image of the day. You can setup a cron job to execute it automatically (or use anacron).
It automatically resize the image to 4k resolution (hardcoded). You also have some dependencies to fulfill.


```bash
crontab -e
#insert this line to execute the script every 10 min
*/10 * * * *   DISPLAY=:0 path/to/ng_wallpaper.py > /tmp/ng_wpp

```

Than i use this image for i3lock. My `blurlock` is something like
```bash
#!/bin/bash
#get last image
i3lock -i $(ls -d -t ~/Pictures/NationalGeographics/* | head -1)
sleep 1
exit 0

```
the config is mainly the Manjaro-i3 one, with some small changes.
