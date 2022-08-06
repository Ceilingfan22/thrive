Thrive Launcher
===============

### [Build Status](https://dev.revolutionarygamesstudio.com/ci/2)

Thrive launcher is a desktop application that manages downloading and
installing the game releases.

For more information, visit [Revolutionary Games' Website](http://revolutionarygamesstudio.com/), 
[Thrive repository](https://github.com/Revolutionary-Games/Thrive).



### Required packages

On Linux a new enough OS is needed to include new enough glibc
version. Latest Ubuntu LTS is the oldest guaranteed distro to work.


### Required windows version

Due to the used framework at least Windows 7 or newer is required.

Releases
--------

Releases are available here:
[Thrive-Launcher releases](https://github.com/Revolutionary-Games/Thrive-Launcher/releases)


Building
--------

If you can't find a precompiled release or you want to develop the
launcher you will need to follow these instructions to build it.

### Dependencies

In order to properly clone this repository you need to make sure you
have [Git LFS](https://git-lfs.github.com/) installed.

You first need dotnet sdk before you can build Thrive Launcher. So
check [here](https://dotnet.microsoft.com/en-us/download)
how to install it.

### Downloading

First clone this repository with `git clone
https://github.com/Revolutionary-Games/Thrive-Launcher.git` now go to
the created directory and run `npm install` this should install all
required packages. You may need to run this again after pulling updates
if your IDE doesn't do so automatically.

### Icons

In order for the icons to work you need to run `./create_icons.rb` to
create all the icon files from the source images. The icon creation
script requires you to
have [ImageMagick](https://www.imagemagick.org/) installed. And as it is written in Ruby
and requires a few gems, you should check the Thrive setup instructions section on that
[here](https://github.com/Revolutionary-Games/Thrive/blob/master/doc/setup_instructions.md#ruby).
Otherwise, running the script most likely fails either due to missing Ruby or a missing gem.

### Running

Now you should have everything set up. You can run Thrive launcher
with `dotnet run` in the Thrive-Launcher directory. Or use a C# IDE to
open the project files to run.

### Issues

If you have issues first make sure that dotnet SDK is properly
installed and you have ran `dotnet restore` in the launcher's folder.


Creating releases
-----------------

TODO: new packaging approach





