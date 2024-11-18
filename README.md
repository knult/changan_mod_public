# changan_mod


Установка
Поочередно вводим команды. Там где запрашивается пароль - вводим adb36987
adb root
adb remount

adb shell mkdir -p /product/overlay
adb shell chmod 755 /product/overlay

adb push /Users/admin/Documents/Changan/install_app_and_russification/test_overlay/Settings_overlay/dist/settings_apps.overlay.apk /product/overlay/
adb push /Users/admin/Documents/Changan/install_app_and_russification/test_overlay/Settings_overlay/dist/settings_internet.overlay.apk /product/overlay/
adb push /Users/admin/Documents/Changan/install_app_and_russification/test_overlay/Settings_overlay/dist/settings_netw.overlay.apk /product/overlay/

adb reboot

включение:
adb shell cmd overlay enable overlay_package_name

отключение:
adb shell cmd overlay disable overlay_package_name

удаление:
adb shell rm /product/overlay/verlay_package_name.apk


: 1 file pushed, 0 skipped. 28.3 MB/s (8530 bytes in 0.000s)


![img.png](changan/sc55pllus_od/fix.tr.ru.incall.commonservice.monday.overlay/before.png "До") ![img.png](changan/sc55pllus_od/fix.tr.ru.incall.commonservice.monday.overlay/after.png "После")


