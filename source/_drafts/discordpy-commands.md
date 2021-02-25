---
title: discord.py 机器人指令
tags: ['discord.py', 'discord', 'bot', '机器人', '开发', 'development']
---

上篇文章讲了discord.py机器人的基本框架，能成功让我们的机器人程序访问Discord API。但是没有机器人命令的机器人真的没意思。所以今天我们来教大家如何制作Discord机器人命令

这是一个命令方法的结构

```python
@bot.command() #声明下面的方法是机器人命令
async def 命令名称 (ctx):
    # 执行命令
```

命令名称要求：和变量名称要求一样

例如

```python
@bot.command()
async def test(ctx):
    # 执行test命令，向服务器频道发送消息
    await ctx.send('test')
```