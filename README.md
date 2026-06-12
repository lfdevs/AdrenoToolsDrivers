# AdrenoTools Driver packages (Freedreno/Turnip CI)

This repository holds scripts and workflow to autobuild new Turnip driver releases adapted for AdrenoTools usage.  
These builds are based on https://github.com/lfdevs/mesa-for-android-container repository (dev/adreno-main).

> [!WARNING]
> Since the modifications made to the upstream Mesa source code on this branch are mainly targeted at Termux:X11, the drivers built using this branch **may not be suitable for scenarios such as game emulators**.

Old README:
<details>
  This is a bash script to build freedreno/turnip for android as a magisk module and an Adreno Tools driver package.

### Scheduled Releases
- Automated releases at 06:00 UTC on the 1st and 15th of each month.

### Notes;

#### Magisk build:
- Root must be visible to target app/game.
- Tested with these apps/games listed [here](list.md).

#### Adreno Tools build:
- Follow application specific instructions to install the driver package.

### To Build Locally
- Obtain the script [turnip_builder.sh](https://raw.githubusercontent.com/ilhan-athn7/freedreno_turnip-CI/main/turnip_builder.sh) on your linux environment. (visit the link and use ```CTRL + S``` keys)
- Execute script on linux terminal ```bash ./turnip_builder.sh```
- To build experimental branchs, change [this](https://github.com/ilhan-athn7/freedreno_turnip-CI/blob/6ef9860e7b755b8b7a83e4ecd398b355a56f9d49/turnip_builder.sh#L11) line, and add one more line to rename unzipped folder to mesa-main.

### References

- https://forum.xda-developers.com/t/getting-freedreno-turnip-mesa-vulkan-driver-on-a-poco-f3.4323871/

- https://gitlab.freedesktop.org/mesa/mesa/-/issues/6802

- https://github.com/bylaws/libadrenotools

</details>

Xclipse support wen eta?
