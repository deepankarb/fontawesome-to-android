# fontawesome-to-android
A python script to convert font awesome icons to png and place them in android density buckets

Forked from [odyniec/font-awesome-to-png](https://github.com/odyniec/font-awesome-to-png)

E.g. to convert all fontawesome icons in green color and place them in hdpi bucket:
```
python fontawtesome-to-android.py ALL --color green --buckets hdpi
```
Or specify HTML colors:
```
python fontawesome-to-android.py ALL --color \#99cc00 --buckets hdpi
```

#Detailed usage
```
usage: fontawesome-to-android.py [-h] [--color COLOR] [--filename FILENAME]
                                 [--font FONT] [--css CSS] [--list]
                                 [--size SIZE] [--margin MARGIN]
                                 [--buckets [BUCKETS [BUCKETS ...]]] [-q]
                                 icon [icon ...]

Exports Font Awesome icons as PNG images.

positional arguments:
  icon                  The name(s) of the icon(s) to export (or "ALL" for all
                        icons)

optional arguments:
  -h, --help            show this help message and exit
  --color COLOR         Color (HTML color code or name, default: black)
  --filename FILENAME   The name of the output file (it must end with ".png").
                        If all files are exported, it is used as a prefix.
  --font FONT           Font file to use (default: fontawesome-webfont.ttf)
  --css CSS             Path to the CSS file defining icon names (instead of
                        the predefined list)
  --list                List available icon names and exit
  --size SIZE           Icon size in pixels for mdpi (default: 32)
  --margin MARGIN       Icon margin in pixels for mdpi
  --buckets [BUCKETS [BUCKETS ...]]
                        The density buckets to generate icons for. Default is
                        mdpi, hdpi, xhdpi, xxhdpi
  -q, --quiet           Suppress output. Any errors are still sent to stderr.
  ```
