---
title: Discord.py 机器人基础框架及申请bot token
date: 2021-02-08 14:29:02
tags: ['discord.py', 'discord', 'bot', '机器人', '开发', 'development']
---

在准备好Discord.py的开发环境之后，我们就可以写属于自己的一个Discord 机器人了。

首先，我们先新建一个py文件，打开

导入discord.py库

```python
    import discord # 导入discord基础库
    from discord.ext import commands #导入discord.ext库中的commands指令集
```

设置客户端和机器人触发前缀，赋值到bot变量

```python
    # command_prefix的字符串为触发前缀，不一定要是感叹号
    bot = commands.Bot(command_prefix="!")
```

使用on_ready()方法，设定运行后的条件

```python
    #设置命令类型为event
    @bot.event
    async def on_ready():
        print('The bot is ready!')
```

最后在文件尾设置`bot.run()`方法，设置bot token让Discord 机器人运行

```python
    # 使用bot.run方法，设置token并运行
    bot.run('bot token here')
```

只要你的网络能访问discord的接口，我们就可以运行机器人了。

下一篇文章我们来教大家如何申请discord的bot token