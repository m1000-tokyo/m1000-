# m1000
m1000.me
# About Me

Hi! I'm a passionate programmer who enjoys exploring multiple areas of software development. From system customization to creative terminal setups, I love pushing the limits of what my tools can do.

You can call me **M1000** — that's my coder handle 👨‍💻.

## 💻 My Setup

- **OS:** Arch Linux (btw 😉)
- **GPU:** NVIDIA GT 730
- **Terminal:** Alacritty or Kitty (depending on the workflow)
- **Shell:** Custom shell configuration
- **System Info Tool:** Neofetch with personalized anime-themed ASCII art
- **Theme:** Anime-inspired ricing project in progress
- **Languages & Tools I Explore:**  
  - Python, JavaScript, Bash, HTML/CSS  
  - C, C++, Rust, Lua  
  - System customization (WM, dotfiles)  
  - Creative use of CLI tools  

## 🎨 Ricing Goals

I'm currently working on a fully anime-themed terminal experience, including:

- Custom ASCII Art for Neofetch
- Anime wallpapers and color schemes
- Tailored prompt and shell aesthetics
- Personalized terminal utilities

## 🎮 Favorite Games

- **Tom Clancy's Rainbow Six Siege**
- **Terraria**
- **Assassin's Creed**
- **FiveM** (GTA V Roleplay)

## 📺 Favorite Anime

- **Tokyo Ghoul**
- **Darling in the Franxx**
- **That Time I Got Reincarnated as a Slime**
- **Solo Leveling**
- **Cyberpunk: Edgerunners**
- **Re:Zero − Starting Life in Another World**

## ❤️ I Love

- Anime (huge fan!)
- Programming across many domains
- Tweaking, customizing, and making my desktop environment truly mine

## 🧠 Sample Advanced Code

Here's a Python example that showcases a custom class-based system with decorators and concurrency — a small peek into how I think as a developer:

```python
import asyncio
from functools import wraps

def log_execution(func):
    @wraps(func)
    async def wrapper(*args, **kwargs):
        print(f"Executing: {func.__name__}")
        result = await func(*args, **kwargs)
        print(f"Finished: {func.__name__}")
        return result
    return wrapper

class TaskManager:
    def __init__(self):
        self.tasks = []

    def add_task(self, coro):
        self.tasks.append(coro)

    async def run_all(self):
        await asyncio.gather(*self.tasks)

@log_execution
async def fetch_data(endpoint):
    await asyncio.sleep(1)
    return f"Data from {endpoint}"

async def main():
    manager = TaskManager()
    endpoints = ["api/user", "api/data", "api/stats"]

    for ep in endpoints:
        manager.add_task(fetch_data(ep))

    await manager.run_all()

if __name__ == "__main__":
    asyncio.run(main())


📬 Contact Me
Feel free to reach out if you want to connect, collaborate, or just talk about code or anime!

Email: contac.m1000@proton.me

Discord: rd_zs

Coder Tag: M1000