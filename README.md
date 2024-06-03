# Where's My Editor?
<p align="center">
<img alt="Where's My Editor? logo" src="src/assets/images/WME_logo.png" width="50%" >
<br>
Logo created by rubice!
</p>
Where's My Editor? is a level editor for the mobile game, Where's My Water? and all it's spinoffs.

NOTE: If you came here to read a .waltex image, then go to [wmwpy](https://github.com/wmw-modding/wmwpy/blob/main/src/wmwpy/utils/waltex.py). `waltex.py` has moved there.

# Get started
To get started: Download "Git" before you follow the steps below: https://www.git-scm.com/downloads

Note: the image below is just a suggestion for those who don't know. Must follow the steps below. Otherwise, it will cause an error.

Step 1. Get the latest release from the [releases tab](https://github.com/SuperHero20101/wheres-my-editor/releases/tag/1.0.0). Extract the zip folder into it's own folder (to keep it's files organized).

Step 2. Next, you need to get the game files. You can get them in many ways, but generally, you want to have the game extracted into a folder, and all the assets in the assets (or Content) folder.

Step 3. Drag the folders "wmwpy" and "wmwpy-0.5.2b0.dist-info" from the folder you extracted: "wheres-my-editor-1.0.0-windows" to the path: "/Lib/site-packages/"

   Note: When installing Python, drag the folders "wmwpy" and "wmwpy-0.5.2b0.dist-info" into the "Python" Data Folder to the path: "/Lib/site-packages/"

   ![Here](https://github.com/SuperHero20101/wheres-my-editor/blob/main/7.png)

Step 4. Open the cmd:

![Here](https://github.com/SuperHero20101/wheres-my-editor/blob/main/5.png)

Step 5. Copy and paste:

1:
```
pip install -r requirements.txt
```
or
```sh
py -m pip install -r requirements.txt
```
2:
```sh
pip install -r requirements-build.txt
```
3:
```sh
pip install wmwpy@git+https://github.com/wmw-modding/wmwpy
```
4. It will open "Where's my Editor?" if you paste in cmd :
```
cd src
python main.py
```
![Here](https://github.com/SuperHero20101/wheres-my-editor/blob/main/6.png)

Step 6. Select the game folder (In "wheres-my-water-1.0.0-windows.zip" there is a game folder available in the "Where's my water" folder).

Step 7. Now you got it up and running.

If you run into any issues, please send a bug report (shortcut in Help > Send bug report, or the issues page in this repository).

# Building
## Setup
In "wheres-my-editor-1.0.0-windows.zip", there is available to build "WME" so just download "Git" and enter the command below.


run
```
pip install -r requirements.txt
```
or
```sh
py -m pip install -r requirements.txt
```

Now, since this is being developed at the same time as [wmwpy](https://github.com/wmw-modding/wmwpy), there will be features I use that are not in a full release yet. If you want to test it out, get wmwpy from github, or update it (this is in the `requirements.txt`)

```sh
pip install wmwpy@git+https://github.com/wmw-modding/wmwpy
```

Once I make a full release, I will also make a wmwpy release, so this is only needed if you want to test the dev version.

---

Start by extracting your where's my water apk file into a directory. When you run the program for the first timze, it'll ask you to select the game directory. This can also be configurable in the `settings.json` file that is generated by the program.

## Build exe
### Install dependencies
To build an exe for wme, you need to install the dependencies.

```sh
pip install -r requirements-build.txt
```

Note: you need `requirements.txt` in the same directory, as this `requirements-build.txt` references `requirements.txt`.

Make sure `wmwpy` is installed from github (you shouldn't need to do this, as `wmwpy` is installed from github in the `requirements.txt`)

```sh
pip install wmwpy@git+https://github.com/wmw-modding/wmwpy
```

### Build exe

```sh
py build.py
```

or

```sh
python build.py
```

The output is in `dis/wme.exe` (if you're not on windows, it probably won't be an exe).

# Todo

- [x] Export `xml` file
- [x] Export `png` file
- [x] Add and remove objects
- [ ] Room object. 
    - This has kind of been implemented, because wmw1 uses the image for the room placement, but the later games use an object (which can be loaded).
- [ ] Complete settings menu
- [ ] Level explorer
- [x] Fix some objects not loading
- [ ] Image editor

# Credits
- Thanks to [rubice!](https://youtube.com/@rubice2022) for creating the logo. I am not skilled enough to make something that looks that good.
- Thanks to [campbellsonic](https://github.com/campbellsonic) for the script to load `waltex` images. I could not have done it without them.

# Special thanks
- Thanks to AwesomeDragon970#8068 for helping debug the program on MacOS. They are very awesome!
