# BlobEditor
A simple raylib + D project. [Watch a video](https://www.youtube.com/watch?v=RIVDdXV6D-A)

### Clone this repository (with all submodules!)

```git clone --recurse-submodules https://github.com/trikko/BlobEditor```

### Compile raylib 3.0.0 (with raygui)

```
cp ext/raygui/src/*.h ext/raylib/src
cd ext/raylib/src/
make PLATFORM=PLATFORM_DESKTOP RAYLIB_MODULE_RAYGUI=TRUE RAYLIB_MODULE_RAYGUI_PATH=../../raygui/src CFLAGS+="-DRAYGUI_SUPPORT_ICONS"
sudo make install PLATFORM=PLATFORM_DESKTOP RAYLIB_MODULE_RAYGUI=TRUE RAYLIB_MODULE_RAYGUI_PATH=../../raygui/src CFLAGS+="-DRAYGUI_SUPPORT_ICONS"
```

### Make sure you have a D compiler installed

To get the best performances, install ldc2. [Here the binary for your platform](https://github.com/ldc-developers/ldc/releases)

Another option is the official D compiler but it generates slower executables. [You can download it from here](https://dlang.org/)

### Compile & run BlobEditor

If you installed ldc2:
```dub --compiler=ldc2 --b=release-nobounds```

if you installed dmd:
```dub  --b=release-nobounds```

