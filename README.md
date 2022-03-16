# Duolingo Module for Polybar
Unofficial module to act as a reminder to do your daily language lessons.

![Duo Module for Polybar](https://cdn.imgchest.com/files/pyq9cpxkq42.png)

## Dependencies
* `pip install duolingo-api`

Recommend to utilize Font Awesome, Siji or similar fonts for the glyphs, although they are technically not required for the module to function.

## Installation
- Place duo.py within your polybar directory. Make sure to include your _username_ and _password_ at the top of the file.
`~/.config/polybar/duo.py`

## Module
```ini
[module/duo]
type = custom/script
exec = python3 $HOME/.config/polybar/duo.py
interval = 600 #adjust as desired
label = %output%
click-left = firefox --new-tab duolingo.com
```
- Place the module where prefered on the bar
```ini
...
modules-center = date duo
...
```
- Lastly make sure to save your config.ini and reload your polybar!

Duolingo-API offers plenty more information for you to use at your discretion. This is merely a simple module with the basics included. There is plenty of room to implement additional features within the python script itself. Have fun with it and happy language learning!
