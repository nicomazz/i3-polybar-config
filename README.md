# i3-polybar-misc-config
My i3 configuration with polybar for HiDPI screen (4k).
![demo image](https://github.com/nicomazz/i3-polybar-config/blob/master/demo.png?raw=true "demo image")
Since I use many computers, the main intent of this repository is to keep my configuration files somewhere.
Even if there is more than only the `i3` and `polybar` configuration, I've decided to keep this title, because is exactly what I was searching for a lot of time ago.
Update: I've recently added the configuration of my other laptop.
![demo image](https://github.com/nicomazz/i3-polybar-config/blob/master/jumper.png?raw=true "demo image")
Here I'll also write about the problems (and the solutions) I've found, putting the code directly in the readme.

## Features:

#### Polybar
- Temperature
- Memory usage
- IP address with dw/up speed
- Volume and luminosity (use mouse wheel to increase or decrease) 
- Battery
- Currently played Spotify song


#### i3
The configuration is pretty similar to the one of Manjaro i3, with some personalization.

#### Rofi
I use `rofi` to start applications and move around opened windows with this options: `rofi -combi-modi window#drun -show combi -modi combi -show-icons`

#### Daily desktop background update and usage in i3lock
`ng_wallpaper.py` update desktop image daily, based on the National geographic image of the day (maybe some additional dependency are needed)

```bash
crontab -e
#insert this line to execute the script every 10 min
*/10 * * * *   DISPLAY=:0 path/to/ng_wallpaper.py > /tmp/ng_wpp
```

Then I use this image for `i3lock`. This is the script I use to launch i3lock:
```bash
#!/bin/bash
#get last image
i3lock -i $(ls -d -t ~/Pictures/NationalGeographics/* | head -1)
sleep 1
exit 0
```
#### vim
I'm absolutely not an expert. The `vimrc` inside the vim folder helps me to be a little bit more productive. There you can also find some notes about commands I usually use, and often forgot about.

## Important
You probably have to replace some path (try `find . -type f  -exec grep -l "path/to" {} \;`)
Inspiration from:
 - [space](https://github.com/jaagr/dots/tree/master/.local/etc/themer/themes/space "Polybar space theme")
 - [spotify](https://github.com/Jvanrhijn/polybar-spotify "Spotify polybar module")
