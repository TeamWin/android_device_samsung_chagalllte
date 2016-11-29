## TWRP device tree for Samsung Galaxy Tab S 10.5 LTE (chagalllte)

Add to `.repo/local_manifests/chagalllte.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/samsung/chagalllte" name="android_device_samsung_chagalllte" remote="TeamWin" revision="android-6.0" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_chagalllte-eng
make -j5 recoveryimage
```

Kernel sources are available at: https://github.com/jcadduono/android_kernel_samsung_universal5420/tree/twrp-6.0
