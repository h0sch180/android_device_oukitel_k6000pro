# Resurrection Remix 5.8.5 device tree for OUKITEL K6000Pro 

Oukitel K6000 Pro(K6000Pro)
============================

![Oukitel K6000 Pro](http://image4.geekbuying.com/ggo_pic/2016-07-04/2016074018415918g6i204.jpg "Oukitel K6000 Pro")

### Specifications

Component Type | Details
-------:|:-------------------------
CPU     | 1.3GHz Octa-Core MT6753
GPU     | Mali-T720
Memory  | 3GB RAM
Shipped Android Version | 6.0.1
Storage | 16GB
Battery | 6000 mAh
Display | 5.5" 1920 x 1080 px DPI 480
Rear Camera | 13MP, Int.13MP (Sony IMX149 Exmor RS)
Front Camera | 5MP, Int. 5MP (OV)

# Instructions
```
repo init -u git://github.com/LineageOS/android.git -b cm-14.1
repo sync
git https://github.com/h0sch180/android_device_oukitel_k6000pro.git device/OUKITEL/K6000Pro
./device/OUKITEL/K6000Pro/patches_mtk/apply-patches.sh
. build/envsetup.sh
export JACK_SERVER_VM_ARGUMENTS="-Dfile.encoding=UTF-8 -XX:+TieredCompilation -Xmx8g"
./prebuilts/sdk/tools/jack-admin kill-server
./prebuilts/sdk/tools/jack-admin start-server
brunch K6000Pro
```

# Acknowledgements

* seluce
* iodine71
* olegsvs
* danielhk
* Zormax
* xcore995
* SRTK
* and others I might have forgotten to include
