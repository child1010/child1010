Run the code below, after replacing the token. 👀
```py
import discord
import random
from discord.ext import commands
TOKEN = 'Token here'

client = commands.Bot(command_prefix="vt!")

@client.event
async def on_ready():
    print("Ready!")
    
@client.command()
async def discord(ctx):
  await ctx.send("vt#4339")
  
@client.command()
async def learning(ctx):
  await ctx.send("nothing lol")
  
@client.command()
async def WIP(ctx):
  await ctx.send("RAI")
  
@client.command()
async def projects(ctx):
  await ctx.send("https://github.com/child1010")
  
@client.command()
async def tools(ctx):
  toolslist = ["Python3", "VS CODE", "nextcord"]
  tools = random.choice(toolslist)
  await ctx.send(tools)
  
client.run(TOKEN)
```
