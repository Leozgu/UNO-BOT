
 # 项目来源[jh0ker/mau_mau_bot](https://github.com/jh0ker/mau_mau_bot)
 
# UNO_CN_Bot

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](./LICENSE)

一个可以在群里玩UNO的Telegram机器人。

创建机器人所需环境：

- Python (3.4+)
- [python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot)
- [Pony ORM](https://ponyorm.com/)

## Setup

- 从[@BotFather](http://telegram.me/BotFather)获取机器人token，并填入`config.json`.
在`locales`文件夹下，执行`compile.sh`，将所有语言文件由`.po`转化为`.mo`.
  或执行: `find . -maxdepth 2 -type d -name 'LC_MESSAGES' -exec bash -c 'msgfmt {}/unobot.po -o {}/unobot.mo' \;`.
- 在BotFather中为机器人启用 `/setinline` 和 `/setinlinefeedback`.
- 安装模块 (建议使用 `virtualenv` ): `pip install -r requirements.txt`

你可以在`config.json`中更改一些游戏参数，如回合时间、最少玩家数量和默认游戏模式

目前可用游戏模式: Classic , Sanic and Wild. （使用 `/modes` 命令查看模式内容）

## Run
执行 `python3 bot.py` 启动机器人.
或者 `nohup python3 bot.py &` 后台运行机器人

## 其他

[详细教程](https://github.com/Leozgu/UNO-BOT/wiki/%E8%AF%A6%E7%BB%86%E6%95%99%E7%A8%8B)
