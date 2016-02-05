## TWRP device tree for l70pn (D290)
------------

### How to setup build environment and compile TWRP for LG L Fino D290:

-------------

Initializing a Build Environment:

    https://source.android.com/source/initializing.html

Initialize repo:

    repo init -u https://github.com/marduk191/recovery_manifest.git -b android-5.1
    repo sync
Swap out the /bootable/recovery branch for the latest one (6.0)

then sync again
Sync this repo to /device/lge/l70pn


-------------

How to build:
    
    make clobber
    . build/envsetup.sh
    lunch omni_l70pn-userdebug
    make -J# recoveryimage
    
" # being the number of cores."


