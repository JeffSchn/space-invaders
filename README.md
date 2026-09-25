# Space Invaders

[![Language](https://img.shields.io/badge/language-python-blue.svg?style=flat)](https://www.python.org)
[![Module](https://img.shields.io/badge/module-pygame-brightgreen.svg?style=flat)](http://www.pygame.org/news.html)
[![Release](https://img.shields.io/badge/release-v1.0-orange.svg?style=flat)](http://www.leejamesrobinson.com/space-invaders.html)

## About

Space Invaders is a two-dimensional fixed shooter game in which the player controls a ship with lasers by moving it horizontally
across the bottom of the screen and firing at descending aliens. The aim is to defeat five rows of ten aliens that move
horizontally back and forth across the screen as they advance towards the bottom of the screen. The player defeats an alien,
and earns points, by shooting it with the laser cannon. As more aliens are defeated, the aliens' movement and the game's music
both speed up.

The aliens attempt to destroy the ship by firing at it while they approach the bottom of the screen. If they reach the bottom,
the alien invasion is successful and the game ends. A special "mystery ship" will occasionally move across the top of the
screen and award bonus points if destroyed. The ship is partially protected by several stationary defense bunkers that are
gradually destroyed by projectiles from the aliens and player.

<img src="http://i.imgur.com/u2mss8o.png" width="300" height="240" />
<img src="http://i.imgur.com/mR81p5O.png" width="300" height="240"/>

## How To Play

- If you don't have [Python](https://www.python.org/downloads/) or [Pygame](http://www.pygame.org/download.shtml) installed, you can simply double click the .exe file to play the game.
  **Note:** _The .exe file needs to stay in the same directory as the sounds, images, and font folders._

- If you have the correct version of Python and Pygame installed, you can run the program in the command prompt / terminal.

```bash
cd SpaceInvaders
python spaceinvaders.py
```

**Note:** If you're using Python 3, replace the command "python" with "python3"

**MacOS Mojave**: You need to use Python 3.7.2 or greater: [Source](https://github.com/pygame/pygame/issues/555)

## Play in the Browser

The game can be compiled to WebAssembly with [pygbag](https://pypi.org/project/pygbag/) and served from a local web server.

```bash
pip install pygbag
cd space-invaders
pygbag --disable-sound-format-error .
```

Then open [http://localhost:8000](http://localhost:8000) and click the page to start. `main.py` is the browser entry point.
The first build downloads the pygbag browser runtime, so it needs internet access.

To produce static files you can host anywhere (GitHub Pages, Azure Static Web Apps, etc.), run
`pygbag --build --disable-sound-format-error .` and deploy the contents of `build/web/`.

**Note:** `--disable-sound-format-error` is needed only because the original `.wav` files are kept for the `.exe`.
The Python code loads the `.ogg` versions, which browsers support.

## Demo

[![Space Invaders](http://img.youtube.com/vi/_2yUP3WMDRc/0.jpg)](http://www.youtube.com/watch?v=_2yUP3WMDRc)

## Notable Forks

- [AI research project where four types of agents control the ship and play the game](https://github.com/scott-pickthorn/Space_Invaders)
- [NEAT program that evolves to beat the game](https://github.com/lairsonm/neat-in-space-invaders)

## Contact

Thanks for checking out my game and I hope you enjoy it! Feel free to contact me.

- Lee Robinson
- lrobinson2011@gmail.com
