## Build TeamWinRecoveryProject(TWRP) for a7y18lte

```bash
// make folders
$ mkdir twrp && cd twrp 
// init the repo 
$ repo init -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git 
// clone my repo
$ git clone https://github.com/samsungexynos7885/android_manifest_samsung_a7y18lte -b twrp .repo/local_manifests
// sync the repo
$ repo sync -j`nproc` --force-sync -c 
// start to the build
$ . build/envsetup.sh && lunch omni_a7y18lte-eng && export ALLOW_MISSIN_DEPENDENCIES=true && mka recoveryimage
```
