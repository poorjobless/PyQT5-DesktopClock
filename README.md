### DesktopClock
___

Desktop Clock (Desktop widget).

Requirements:
- Python 3.6
- PyQt5
- pymodbus
- numpy

![](doc/screen1.png)
**fig1. Widget**

![System Tray](doc/screen2.png)
**fig2. System Tray**

更新说明：

1. 添加 Suncalc 用于计算天文时间
2. 添加 edge-tts 用于实现语音报时
3. 添加 模拟时钟 实现数字/模拟双时钟

___
### How to create virtual environment
**Windows**
~~~bash
$ python -m venv env
$ source env/Scripts/activate
(env)$ python -m pip install --upgrade pip
(env)$ pip install -r requirements.txt
(env)$ deactivate
~~~
**Linux**
~~~bash
$ python3 -m venv env
$ source env/bin/activate
(env)$ python -m pip install --upgrade pip
(env)$ pip install -r requirements.txt
(env)$ deactivate
~~~
#### Executable file creation
**Windows** (DesktopClock.exe)
~~~bash
$ source env/Scripts/activate
(env)$ pyinstaller --clean --onefile --noconsole --icon=clock.ico --name DesktopClock ./main.py
(env)$ cp -r ./images dist/
(env)$ deactivate
~~~
**Linux**
~~~bash
$ source env/bin/activate
(env)$ pyinstaller --clean --onefile --noconsole --icon=clock.ico --name DesktopClock ./main.py
(env)$ cp -r ./images dist/
(env)$ deactivate
~~~
---
### How to use
~~~bash
$ source env/Scripts/activate
(env)$ python main.py
~~~
