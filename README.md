# linuxdeploy-plugin-ncurses

This is an (as of yet experimental) plugin for linuxdeploy. Its job is to bundle additional resources for applications that use ncurses.


## Usage

```bash
# get linuxdeploy and linuxdeploy-plugin-ncurses
> wget -c "https://raw.githubusercontent.com/linuxdeploy/linuxdeploy-plugin-ncurses/master/linuxdeploy-plugin-ncurses.sh"
> wget -c "https://github.com/linuxdeploy/linuxdeploy/releases/download/continuous/linuxdeploy-x86_64.AppImage"

# first option: install your app into your AppDir via `make install` etc.
# second option: bundle your app's main executables manually
# see https://docs.appimage.org/packaging-guide/from-source/native-binaries.html for more information
> [...]

# call through linuxdeploy
> ./linuxdeploy-x86_64.AppImage --appdir AppDir --plugin ncurses --output appimage
```
