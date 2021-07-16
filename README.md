# Description

Turns three files [like this](https://jsfiddle.net/5no9wqkd/2/) (or any svgs)
Into [this](https://jsfiddle.net/samgermain/caqtpkbj/)

# How to use

In `create-svg-animation.py`, near the bottom, replace the filenames with the filenames of your svgs. The number to the right is how many miliseconds the animations lasts while transitioning to that image

```
svgs = [
    ["./trombone.svg", 1000],
    ["./trombone2.svg", 1000],
    ["./trombone3.svg", 1000],
    ["./trombone4.svg", 1000],
]
```

Replace the value stored in `output` with the filename you want for the svg animation

```
output="trombone-anim.svg"
```

Run the following in the command line

```
python -m pip install bs4 lxml
python main.py
```

--------------------

You may need to remove these lines from your svgs

```
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN" "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
```

# Limitations

Currently this only produces looping animations