# VoidUI Eternity Project #
# Early Development #
# // FPush Warning // #

![void_Frame2](https://user-images.githubusercontent.com/34755141/173379206-ea461b24-321e-4186-b3d4-2bfbae6872d4.jpg)

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/VoidUI/manifest -b aosp-12.1

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```