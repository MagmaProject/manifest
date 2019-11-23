To initialize your local repository, use this command:

	repo init -u https://github.com/MagmaProject/manifest.git -b ten

 Then to sync up:

```bash
repo sync --force-sync --no-tags --no-clone-bundle -j$(nproc --all)
```

Build Magma
==================

```bash
source build/envsetup.sh
   
lunch magma_codename-buildtype
   
mka magma
```
