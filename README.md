# Duolingo Module for Polybar
Simplistic module to act as a reminder to do your daily lessons as well as a motivational streak counter.

### Requires

```sh
pip install duolingo-api
```
Recommend to utilize Font Awesome, Siji or similar fonts for the glyphs, although they are technically not required for the module to function.

### Installation
- First place duo.py within your polybar directory. Make sure to include your _username_ and _password_ at the top.
```
~/.config/polybar/duo.py
```
- Then modify your polybar config.ini
```
[module/duo]
type = custom/script
exec = python3 $HOME/.config/polybar/duo.py
interval = 600 #adjust as desired
label = %output%
click-left = firefox --new-tab duolingo.com
```
- Place the module where prefered on the bar
```
modules-center = date duo
```
- Lastly make sure to save your config.ini and reload your polybar!

Duolingo-API offers plenty more information for you to use at your discretion. This is merely a simple module with the basics included. There is plenty of room to implement additional features within the python script itself. Have fun with it and happy language learning!
