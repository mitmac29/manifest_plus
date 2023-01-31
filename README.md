<p align="center">
<img src="https://raw.githubusercontent.com/AospExtended/Documentation_and_thread-template/10.x/Banner.png" > 
</p>

Aex AfterLife Version.
===========
AfterLife is an external version of aex, since aex announced that the project was temporarily suspended until an unspecified time,
we are fans of aex who don't want aex to stop trying to continue this project,
and of course in our hearts aex never dies.

Credits
-------
* [**JDCTeam**](https://github.com/AOSP-JF-MM)
* [**DirtyUnicorns**](https://github.com/DirtyUnicorns)
* [**TeamSubstratum (Theme Engine)**](https://github.com/Substratum)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
* [**Nitrogen Project**](https://github.com/nitrogen-project)
* [**ABC ROM**](https://github.com/ezio84)
* [**GZOSP**](https://github.com/GZOSP)
* [**Pure Nexus**](https://github.com/PureNexusProject)
* [**OmniROM**](https://github.com/omnirom/)
* [**AOSPA**](https://github.com/aospa/)
* [**BlissRoms**](https://github.com/BlissRoms)
* [**WizardPrjkt**](https://t.me/wizardX00T)

How to Build?
-------------

To initialize your local repository using the AospExtended trees, use a 
command like this:

```bash
repo init -u https://github.com/AfterLifePrjkt/manifest_plus.git -b 12L
```
To initialize a shallow clone, which will save even more space & time, use a command like this:

```bash
repo init --depth=1 -u https://github.com/AfterLifePrjkt/manifest_plus.git -b 12L
```

Then to sync up:
----------------

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
Finally to build:
-----------------

```bash
source build/envsetup.sh
lunch aosp_device_codename-userdebug
m aex -j$(nproc --all) | tee log.txt
```
