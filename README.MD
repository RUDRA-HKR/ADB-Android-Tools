Termux mein ADB (Android Debug Bridge) ka use karke aap Android device ko control kar sakte hain. Yahaan kuch basic commands hain jo Termux mein ADB ke liye use kiye ja sakte hain:

**ADB Android Tools Installation:**
1. `apt update && apt upgrade -y`
2. `pkg install android-tools` & `pkg install adb`
3. `adb version` is `ADB Version`

1. **Connected Devices ko List karna:**
   ```
   adb devices
   ```
   Yeh command connected devices ki list dikhata hai.

2. **Wireless Mode par Device ko Connect karna:**
   ```
   adb tcpip 5555
   ```
   Wireless mode mein device ko connect karne ke liye ye command use hoti hai.

3. **Device ko Connect karna:**
   ```
   adb connect DEVICE_IP:5555
   ```
   Wireless mode mein device ko connect karne ke liye, yahan "DEVICE_IP" device ka IP address hota hai.

4. **File Transfer:**
   ```
   adb pull DEVICE_FILE_PATH LOCAL_PATH
   adb push LOCAL_FILE_PATH DEVICE_PATH
   ```
   File transfer ke liye `adb pull` aur `adb push` commands ka use hota hai.

5. **App Management:**
   ```
   adb install app.apk
   adb uninstall com.example.app
   ```
   App installation aur uninstallation ke liye `adb install` aur `adb uninstall` commands use kiye ja sakte hain.

6. **Screen Capture:**
   ```
   adb shell screencap /sdcard/screenshot.png
   ```
   Device ki screenshot leta hai aur specified location par save karta hai.

7. **Device Info:**
   ```
   adb shell getprop
   adb shell cat /proc/cpuinfo
   ```
   Device ke properties aur CPU information ko display karta hai.

8. **IMEI aur Serial Number:**
   ```
   adb shell service call iphonesubinfo 1
   adb shell getprop ro.serialno
   ```
   Device ka IMEI number aur serial number display karta hai.

9. **Wi-Fi Management:**
   ```
   adb shell svc wifi enable
   adb shell svc wifi disable
   ```
   Wi-Fi ko enable aur disable karne ke liye use hota hai.

10. **Device Reboot/Shut Down:**
   ```
   adb reboot
   adb reboot recovery
   adb reboot bootloader
   adb shell reboot -p
   ```
   Device ko restart aur shutdown karne ke liye use hota hai.

11. **Battery Information:**
   ```
   adb shell dumpsys battery
   ```
   Device ki battery status aur information ko display karta hai.

12. **Network Information:**
   ```
   adb shell netstat
   adb shell ping
   ```
   Network connections aur ping responses ko display karta hai.

13. **Package Management:**
   ```
   adb shell pm list packages
   adb shell pm clear PACKAGE_NAME
   ```
   Installed packages ki list ko show karta hai aur specific app ka data clear karta hai.

14. **CPU Usage:**
   ```
   adb shell top
   ```
   CPU usage ko display karta hai.

15. **Device Screenshot:**
   ```
   adb shell screencap /sdcard/screenshot.png
   ```
   Device ki screenshot leta hai aur specified location par save karta hai.

16. **SELinux Status:**
   ```
   adb shell getenforce
   ```
   Device ke SELinux enforcement status ko show karta hai.

17. **Clipboard Access:**
   ```
   adb shell input text "TEXT"
   adb shell input keyevent KEYCODE
   ```
   Device ke clipboard mein text input karta hai aur keyboard ke keys ko simulate karta hai.

18. **Sensor Information:**
   ```
   adb shell dumpsys sensorservice
   ```
   Device ke sensors ki information ko display karta hai.

19. **Package Installation from APK:**
   ```
   adb install app.apk
   ```
   APK file ko device mein install karne ke liye use hota hai.

20. **Logcat:**
   ```
   adb logcat
   ```
   Device ke logs ko live stream karta hai, jisse debugging aur troubleshooting kiya ja sakta hai.

21. **Backup and Restore:**
   ```
   adb backup
   adb restore
   ```
   Device data ka backup lena aur restore karna.

22. **Key Event Emulation:**
   ```
   adb shell input keyevent KEYCODE
   ```
   Device par virtual key event generate karna, jaise ki home button press karna, back button press karna, etc.

23. **USB Debugging Toggle:**
   ```
   adb shell settings put global adb_enabled 1
   adb shell settings put global adb_enabled 0
   ```
   USB debugging ko enable aur disable karna.

24. **Battery Statistics:**
   ```
   adb shell dumpsys batterystats
   ```
   Battery statistics aur details ko display karna.

25. **Package Information:**
   ```
   adb shell dumpsys package PACKAGE_NAME
   ```
   Specific app ki information aur details ko display karna.

26. **Device Info:**
   ```
   adb shell getprop
   adb shell cat /proc/cpuinfo
   ```
   Device ke properties aur CPU information ko display karta hai.

27. **IMEI aur Serial Number:**
   ```
   adb shell service call iphonesubinfo 1
   adb shell getprop ro.serialno
   ```
   Device ka IMEI number aur serial number display karta hai.

28. **Wi-Fi Management:**
   ```
   adb shell svc wifi enable
   adb shell svc wifi disable
   ```
   Wi-Fi ko enable aur disable karne ke liye use hota hai.

29. **Device Reboot/Shut Down:**
   ```
   adb reboot
   adb reboot recovery
   adb reboot bootloader
   adb shell reboot -p
   ```
   Device ko restart aur shutdown karne ke liye use hota hai.

Join My Telegram Channel <storage><a>https://t.me/RUDRA_HKR0<a><storage></details>
