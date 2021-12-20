
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
  ctx.send("JavaScript")
  
@client.command()
async def WIP(ctx):
  ctx.send("MemeAPI")
  
@client.command()
async def projects(ctx):
  ctx.send("https://github.com/child1010")
  
@client.command()
async def fact(ctx):
  facts = ["Most annoying person on this earth", "Idiot", "cool"]
  randfact = random.choice(facts)
  await ctx.send(randfact)
  
@client.command()
async def tools(ctx):
  tools = ["Python3", "IDLE", "Discord.py"]
  await ctx.send(tools)
  
client.run(TOKEN)
```
