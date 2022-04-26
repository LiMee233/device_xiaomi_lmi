# Device Tree for Xiaomi lmi devices

The Redmi K30 Pro / POCO F2 Pro (codenamed "lmi") is a flagship smartphone from Xiaomi announced in March 2020.

## Device specifications

| Device                  | Redmi K30 Pro / POCO F2 Pro                                     |
| ----------------------: | :-------------------------------------------------------------- |
| SoC                     | Qualcomm SM8250 Snapdragon 865                                  |
| CPU                     | 1x2.84 GHz Kryo 585 & 3x2.42 GHz Kryo 585 & 4x1.80 GHz Kryo 585 |
| GPU                     | Adreno 650                                                      |
| Memory                  | 6GB / 8GB / 12GB                                                |
| Shipped Android version | Android 10, MIUI 11                                             |
| Storage                 | 128GB / 256GB / 512GB                                           |
| Battery                 | Li-Po 4700 mAh, non-removable                                   |
| Dimensions              | 163.3 x 75.4 x 8.9 mm                                           |
| Display                 | 1080 x 2400 pixels, 6.67 inches                                 |
| Rear camera 1           | 64 MP, Dual-LED dual-tone flash, HDR, panorama                  |
| Rear camera 2           | 5 MP (Std) / 8 MP (Pro)                                         |
| Rear camera 3           | 13 MP                                                           |
| Rear camera 4           | 2 MP                                                            |
| Front camera            | Motorized pop-up 20 MP, HDR                                     |


## Device picture

![Redmi K30 Pro / POCO F2 Pro](https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/46f95bd552fa134820a7daea19e507ef.png)

## Build guide

1. Fllow the [manifest](https://github.com/PixelExperience/manifest/tree/twelve) of Pixel Experience to sync.
2. Clone [device_xiaomi_lmi](https://github.com/LiMee233/device_xiaomi_lmi/tree/twelve) into `device/xiaomi/lmi`.
3. Clone [device_xiaomi_sm8250-common](https://github.com/LiMee233/device_xiaomi_sm8250-common/tree/twelve-lmi) into `device/xiaomi/sm8250-common`.
8. Clone [device_xiaomi_sm8250-extras](https://github.com/PixelExperience-Devices/device_xiaomi_sm8250-extras/tree/twelve) into `device/xiaomi/sm8250-extras`.
4. Clone [kernel_xiaomi_sm8250](https://github.com/LiMee233/kernel_xiaomi_sm8250/tree/twelve-lmi) into `kernel/xiaomi/sm8250`.
5. Clone [vendor_xiaomi_sm8250-common](https://github.com/LiMee233/vendor_xiaomi_sm8250-common/tree/twelve-lmi) into `vendor/xiaomi/sm8250-common`.
6. Clone [vendor_xiaomi_lmi](https://gitlab.com/the-muppets/proprietary_vendor_xiaomi/-/tree/lineage-19.1/lmi) into `vendor/xiaomi/lmi`.
7. Clone [hardware_xiaomi](https://github.com/PixelExperience/hardware_xiaomi/tree/twelve) into `hardware/xiaomi`.
9. Fllow the [manifest](https://github.com/PixelExperience/manifest/tree/twelve) of Pixel Experience to build.

## Modify upstream source code

### Fix Camera and touchlight

Pick [this](https://review.arrowos.net/c/ArrowOS/android_system_libhwbinder/+/14833).
