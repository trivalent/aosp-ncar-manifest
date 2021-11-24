
The project is based on latest 11 AOSP release (`android-11.0.0_r48`) because latest 12 AOSP releases (up to r15) have problem with `aosp_car_x86` emulator startup.

## Requirements to host PC
[Link to HW and SW requirements from Google.](https://source.android.com/setup/build/requirements)

## Setup and sync project
```
$ mkdir ncar && cd ncar
$ repo init -u git@github.com:nkh-lab/aosp-ncar-manifest.git
$ repo sync -c -d
```

## Build
```
$ . ./build/envsetup.sh
$ lunch ncar_x86-userdebug
$ make
```

## Run
```
$ emulator
```
