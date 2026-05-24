🎮 Games Launcher – a stylish game launcher for Windows

[⬇️ Go to Download](#download-section)

[⬇️ Go to Games Launcher Screenshot](#GamesLauncherScreenshot-section)

Hi! 👋 This is my first programming project, created with great passion and nightly coding sessions. I wanted to create something that would make managing and launching games a truly enjoyable experience – with smooth animations, a clean design, and clever little features that I've always missed in other tools.

Since this is my debut project, I'm sure there's room for improvement. If you have ideas for new features, spotted a bug, or simply want to suggest an improvement – ​​please contact me! I'd love to continue developing Games Launcher with the community's help.

Launching
Download the .exe file > run GAMES.exe > enjoy the launcher!
On first launch, point the app at your games folder! – and you're done.

⌨️Description:
Turn your `.lnk` shortcuts folder into a beautiful, animated tab grid. Launch games with a single click, track play time, combine background apps, and customize every visual detail.

✨ What it does

🗂 Game Library
Scans the selected folder for `.lnk` shortcuts and displays them in clear tabs. Add custom files (e.g., executables, documents), hide unnecessary titles, and restore them at any time. Icons are extracted from `.exe` files (using `icoextract`) and cached in PNG format – you can also set your own icon.

🔍 Search and Sort
Filter live games by entering part of the name. Sort alphabetically, by number of launches, or by play time – ascending or descending.

🚀 Launch and Statistics
Click a tab – the game launches and the launcher minimizes. When you close the game, your session time is automatically saved and the launch counter increases. Each tab shows, for example, "Launches: 15" and "Game time: 12 hrs 30 mins." This protection prevents two games from running simultaneously.

🧩 IF‑TOO Rules
Need a voice app, overlay, or additional program to start a game? Create a rule: select your main game and a list of background apps. Enable or disable each rule with a toggle—no need to delete it. Manage everything in a dedicated sidebar.

🎨 Themes and RGB Animation
Two built-in themes—dark and light—plus an automatic mode that switches between them at selected times. The title, search frames, game names, and the gamepad icon smoothly change rainbow colors. Hover over a tab and it will slightly enlarge and highlight.

🖼 Background
Set a single image or a folder of images—the launcher will randomly select one. Right-click on the desktop to go to the next or previous background. You can also remove the background completely.

📏 Dynamic Tab Scaling
By default, tabs are displayed 10% smaller than their base size. Enlarge them with `↑` or `Ctrl + Scroll Up`, and reduce them with `↓` or `Ctrl + Scroll Down`. The scale works smoothly from 0.5× to 2.0×, and icons, fonts, and spacing scale proportionally.

🌐 Five Languages
English (default), Polish, German, Spanish, and Simplified Chinese. Switch via the settings menu.

⌨️ Keyboard and Mouse Shortcuts
| Action | Shortcut |
|---------|---------|
| Scroll through the game list | Mouse wheel |
| Enlarge tabs | `↑` or `Ctrl + Scroll Up` |
| Shrink tabs | `↓` or `Ctrl + Scroll Down` |
| Next Background (Folder) | Right-click → Next Background |
| Previous Background (Folder) | Right-click → Previous Background |

Scaling shortcuts are disabled when typing in the search box or dropdown list.

💾 Portable and persistent
No installation required – run from disk. All settings, statistics, and rules are stored in `%APPDATA%\GRY_Launcher` as readable JSON and TXT files. 🧰 Configuration Files
- `launcher_config.txt` – path to the games folder
- `launcher_main_folder.txt` – path to the main folder
- `launcher_theme_settings.json` – theme mode and schedule
- `launcher_rules.json` – IF‑THEN rules, hidden games, statistics
- `game_icons_cache/` – PNG icon cache folder

📥If you want to create your own executable
You need a Windows system with Python 3.8 or later, an x.py file that you can convert to an 'executable', and the following libraries:

```bash
pip install pillow psutil pywin32 icoextract
```
Building the 'exe' (use PyInstaller) in cmd, type:
```bash
python -m PyInstaller --clean --noconsole --onefile --name "(filename)" --hidden-import=psutil --hidden-import=pythoncom --hidden-import=pywintypes --hidden-import=win32timezone --hidden-import=icoextract --collect-submodules win32com --collect-all PIL --collect-all icoextract (filename).py
```
Example:
`python -m PyInstaller --clean --noconsole --onefile --name "GRY" --hidden-import=psutil --hidden-import=pythoncom --hidden-import=pywintypes --hidden-import=win32timezone --hidden-import=icoextract --collect-submodules win32com --collect-all PIL --collect-all icoextract GRY.py
`
## Download <a name="download-section"></a>
**Suggested**> You can download the compiled ready `.exe` file from [Google Drive](https://drive.google.com/file/d/1aGEXUS5mM01ou7JT8N00c5GxQqn6wJyd/view?usp=sharing).

**Alternatively**> (note: PyInstaller required) You can download the `GAMES.py` file from [Google Drive](https://drive.google.com/file/d/1bJxfXT3ZQGM1CQpycDVmEt3cL7kk1Oep/view?usp=sharing).

You can download the `source code` file from [Google Drive](https://drive.google.com/file/d/1gblu50UZz0h5z64bRjRnG7evxHx6Fj6P/view?usp=sharing).

You can download the `readme` file from [Google Drive](https://drive.google.com/file/d/12LYoeNZ6erTKVA2MckVLEPyoOOh0Zmmn/view?usp=sharing).


*****Games Launcher Screenshot*****: <a name="GamesLauncherScreenshot-section"></a>
![Tekst alternatywny](https://github.com/Emett-S/Games-Launcher/blob/d24e7949992bf66210d9df34fce61062198ae713/Games%20Launcher%20Screenshot_0.png)

![Tekst alternatywny](https://github.com/Emett-S/Games-Launcher/blob/d24e7949992bf66210d9df34fce61062198ae713/Games%20Launcher%20Screenshot_1.png)

![Tekst alternatywny](https://github.com/Emett-S/Games-Launcher/blob/d24e7949992bf66210d9df34fce61062198ae713/Games%20Launcher%20Screenshot_2.png)
