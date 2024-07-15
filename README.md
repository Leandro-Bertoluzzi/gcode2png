# gcode2png

python script for 3d rendering gcode files with mayavi

all images are created with width of 800px and somewhat ~600px height

## Installation:
```bash
sudo pip install -r requirements.txt
```

# Usage:

## Single file generation
```bash
python ./gcode2png.py test.gcode moves=[true/false] support=[true/false] show=[true/false] bed=[true/false]
```

- moves: show movements in red; default=false
- support: show support layers in grey; default=true
- bed: show printbed; default=true
- show: true = show rendered image; false = save rendered image as png file

## batch generation
```bash
python ./gcode2png.py batch /path/to/files/ moves=[true/false] support=[true/false] show=[true/false] bed=[true/false]
```

## Single file parsing
```bash
python ./gcodeParser.py test.gcode
```
Useful for debugging, output will be exported to `parsed.json`.

## Thanks to:
gcodeParser.py forked and modifed from: https://github.com/jonathanwin/yagv
