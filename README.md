This is an old copy of androVM source code.

---------------------------------------------------
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

  <remote  name="aosp"
           fetch="https://android.googlesource.com" />
  <remote  name="androvm"
           fetch="./" />
  <default revision="refs/tags/android-4.1.1_r6.1"
           remote="aosp"
           sync-j="4" />

  <project path="build" remote="androvm" name="platform_build" revision="androVM-4.1.1_r6.1" >
    <copyfile src="core/root.mk" dest="Makefile" />
  </project>
  <project path="abi/cpp" name="platform/abi/cpp" />
  <project path="bionic" remote="androvm" name="platform_bionic" revision="androVM-4.1.1_r6.1" />
  <project path="bootable/bootloader/legacy" name="platform/bootable/bootloader/legacy" />
  <project path="bootable/diskinstaller" remote="androvm" name="platform_bootable_diskinstaller" revision="androVM-4.1.1_r6.1" />
  <project path="bootable/recovery" name="platform/bootable/recovery" />
  <project path="cts" name="platform/cts" />
  <project path="dalvik" remote="androvm" name="platform_dalvik" revision="androVM-4.1.1_r6.1" />
  <project path="development" name="platform/development" />
  <project path="device/asus/grouper" name="device/asus/grouper" />
  <project path="device/common" name="device/common" />
  <project path="device/generic/armv7-a-neon" name="device/generic/armv7-a-neon" />
  <project path="device/generic/armv7-a" name="device/generic/armv7-a" />
  <project path="device/generic/goldfish" name="device/generic/goldfish" />
  <project path="device/google/accessory/arduino" name="device/google/accessory/arduino" />
  <project path="device/google/accessory/demokit" name="device/google/accessory/demokit" />
  <project path="device/moto/common" name="device/moto/common" />
  <project path="device/moto/stingray" name="device/moto/stingray" />
  <project path="device/moto/wingray" name="device/moto/wingray" />
  <project path="device/sample" name="device/sample" />
  <project path="device/samsung/crespo" name="device/samsung/crespo" />
  <project path="device/samsung/crespo4g" name="device/samsung/crespo4g" />
  <project path="device/samsung/maguro" name="device/samsung/maguro" />
  <project path="device/samsung/toro" name="device/samsung/toro" />
  <project path="device/samsung/torospr" name="device/samsung/torospr" />
  <project path="device/samsung/tuna" name="device/samsung/tuna" />
  <project path="device/ti/panda" name="device/ti/panda" />
  <project path="docs/source.android.com" name="platform/docs/source.android.com" />
  <project path="external/aac" name="platform/external/aac" />
  <project path="external/android-mock" name="platform/external/android-mock" />
  <project path="external/antlr" name="platform/external/antlr" />
  <project path="external/apache-harmony" name="platform/external/apache-harmony" />
  <project path="external/apache-http" name="platform/external/apache-http" />
  <project path="external/apache-xml" name="platform/external/apache-xml" />
  <project path="external/astl" name="platform/external/astl" />
  <project path="external/bison" name="platform/external/bison" />
  <project path="external/blktrace" name="platform/external/blktrace" />
  <project path="external/bluetooth/bluez" name="platform/external/bluetooth/bluez" />
  <project path="external/bluetooth/glib" name="platform/external/bluetooth/glib" />
  <project path="external/bluetooth/hcidump" name="platform/external/bluetooth/hcidump" />
  <project path="external/bouncycastle" name="platform/external/bouncycastle" />
  <project path="external/bsdiff" name="platform/external/bsdiff" />
  <project path="external/bzip2" name="platform/external/bzip2" />
  <project path="external/checkpolicy" name="platform/external/checkpolicy" />
  <project path="external/chromium" name="platform/external/chromium" />
  <project path="external/chromium-trace" name="platform/external/chromium-trace" />
  <project path="external/cibu-fonts" name="platform/external/cibu-fonts" />
  <project path="external/clang" name="platform/external/clang" />
  <project path="external/compiler-rt" name="platform/external/compiler-rt" />
  <project path="external/dbus" name="platform/external/dbus" />
  <project path="external/dexmaker" name="platform/external/dexmaker" />
  <project path="external/dhcpcd" name="platform/external/dhcpcd" />
  <project path="external/dnsmasq" name="platform/external/dnsmasq" />
  <project path="external/doclava" name="platform/external/doclava" />
  <project path="external/dropbear" name="platform/external/dropbear" />
  <project path="external/e2fsprogs" name="platform/external/e2fsprogs" />
  <project path="external/easymock" name="platform/external/easymock" />
  <project path="external/eclipse-basebuilder" name="platform/external/eclipse-basebuilder" />
  <project path="external/eclipse-windowbuilder" name="platform/external/eclipse-windowbuilder" />
  <project path="external/elfutils" name="platform/external/elfutils" />
  <project path="external/embunit" name="platform/external/embunit" />
  <project path="external/emma" name="platform/external/emma" />
  <project path="external/esd" name="platform/external/esd" />
  <project path="external/expat" name="platform/external/expat" />
  <project path="external/eyes-free" name="platform/external/eyes-free" />
  <project path="external/fdlibm" name="platform/external/fdlibm" />
  <project path="external/flac" name="platform/external/flac" />
  <project path="external/freetype" name="platform/external/freetype" />
  <project path="external/fsck_msdos" name="platform/external/fsck_msdos" />
  <project path="external/ganymed-ssh2" name="platform/external/ganymed-ssh2" />
  <project path="external/gcc-demangle" name="platform/external/gcc-demangle" />
  <project path="external/genext2fs" name="platform/external/genext2fs" />
  <project path="external/giflib" name="platform/external/giflib" />
  <project path="external/google-diff-match-patch" name="platform/external/google-diff-match-patch" />
  <project path="external/grub" remote="androvm" name="platform_external_grub" revision="androVM-4.1.1_r6.1" />
  <project path="external/gtest" name="platform/external/gtest" />
  <project path="external/guava" name="platform/external/guava" />
  <project path="external/hamcrest" name="platform/external/hamcrest" />
  <project path="external/harfbuzz" name="platform/external/harfbuzz" />
  <project path="external/hyphenation" name="platform/external/hyphenation" />
  <project path="external/icu4c" name="platform/external/icu4c" />
  <project path="external/iproute2" name="platform/external/iproute2" />
  <project path="external/ipsec-tools" name="platform/external/ipsec-tools" />
  <project path="external/iptables" name="platform/external/iptables" />
  <project path="external/javasqlite" name="platform/external/javasqlite" />
  <project path="external/javassist" name="platform/external/javassist" />
  <project path="external/jdiff" name="platform/external/jdiff" />
  <project path="external/jhead" name="platform/external/jhead" />
  <project path="external/jmdns" name="platform/external/jmdns" />
  <project path="external/jmonkeyengine" name="platform/external/jmonkeyengine" />
  <project path="external/jpeg" name="platform/external/jpeg" />
  <project path="external/jsilver" name="platform/external/jsilver" />
  <project path="external/jsr305" name="platform/external/jsr305" />
  <project path="external/junit" name="platform/external/junit" />
  <project path="external/kernel-headers" name="platform/external/kernel-headers" />
  <project path="external/libffi" name="platform/external/libffi" />
  <project path="external/libgsm" name="platform/external/libgsm" />
  <project path="external/liblzf" name="platform/external/liblzf" />
  <project path="external/libmtp" name="platform/external/libmtp" />
  <project path="external/libnfc-nxp" name="platform/external/libnfc-nxp" />
  <project path="external/libnl-headers" name="platform/external/libnl-headers" />
  <project path="external/libpcap" name="platform/external/libpcap" />
  <project path="external/libphonenumber" name="platform/external/libphonenumber" />
  <project path="external/libpng" name="platform/external/libpng" />
  <project path="external/libselinux" name="platform/external/libselinux" />
  <project path="external/libsepol" name="platform/external/libsepol" />
  <project path="external/libusb" name="platform/external/libusb" />
  <project path="external/libusb-compat" name="platform/external/libusb-compat" />
  <project path="external/libvpx" name="platform/external/libvpx" />
  <project path="external/libxml2" name="platform/external/libxml2" />
  <project path="external/libxslt" name="platform/external/libxslt" />
  <project path="external/libyuv" name="platform/external/libyuv" />
  <project path="external/linux-tools-perf" name="platform/external/linux-tools-perf" />
  <project path="external/littlemock" name="platform/external/littlemock" />
  <project path="external/llvm" name="platform/external/llvm" />
  <project path="external/lohit-fonts" name="platform/external/lohit-fonts" />
  <project path="external/markdown" name="platform/external/markdown" />
  <project path="external/mdnsresponder" name="platform/external/mdnsresponder" />
  <project path="external/mesa3d" name="platform/external/mesa3d" />
  <project path="external/mksh" name="platform/external/mksh" />
  <project path="external/mockwebserver" name="platform/external/mockwebserver" />
  <project path="external/mtpd" name="platform/external/mtpd" />
  <project path="external/naver-fonts" name="platform/external/naver-fonts" />
  <project path="external/netcat" name="platform/external/netcat" />
  <project path="external/netperf" name="platform/external/netperf" />
  <project path="external/neven" name="platform/external/neven" />
  <project path="external/nist-sip" name="platform/external/nist-sip" />
  <project path="external/oauth" name="platform/external/oauth" />
  <project path="external/opencv" name="platform/external/opencv" />
  <project path="external/openfst" name="platform/external/openfst" />
  <project path="external/openssh" name="platform/external/openssh" />
  <project path="external/openssl" name="platform/external/openssl" />
  <project path="external/oprofile" name="platform/external/oprofile" />
  <project path="external/ping" name="platform/external/ping" />
  <project path="external/ping6" name="platform/external/ping6" />
  <project path="external/ppp" name="platform/external/ppp" />
  <project path="external/proguard" name="platform/external/proguard" />
  <project path="external/protobuf" name="platform/external/protobuf" />
  <project path="external/qemu" name="platform/external/qemu" />
  <project path="external/qemu-pc-bios" name="platform/external/qemu-pc-bios" />
  <project path="external/quake" name="platform/external/quake" />
  <project path="external/regex-re2" name="platform/external/regex-re2" />
  <project path="external/replicaisland" name="platform/external/replicaisland" />
  <project path="external/safe-iop" name="platform/external/safe-iop" />
  <project path="external/sepolicy" name="platform/external/sepolicy" />
  <project path="external/skia" name="platform/external/skia" />
  <project path="external/smali" name="platform/external/smali" />
  <project path="external/sonivox" name="platform/external/sonivox" />
  <project path="external/speex" name="platform/external/speex" />
  <project path="external/sqlite" name="platform/external/sqlite" />
  <project path="external/srec" name="platform/external/srec" />
  <project path="external/srtp" name="platform/external/srtp" />
  <project path="external/stlport" name="platform/external/stlport" />
  <project path="external/strace" name="platform/external/strace" />
  <project path="external/stressapptest" name="platform/external/stressapptest" />
  <project path="external/svox" name="platform/external/svox" />
  <project path="external/tagsoup" name="platform/external/tagsoup" />
  <project path="external/tcpdump" name="platform/external/tcpdump" />
  <project path="external/tinyalsa" name="platform/external/tinyalsa" />
  <project path="external/tinyxml" name="platform/external/tinyxml" />
  <project path="external/tremolo" name="platform/external/tremolo" />
  <project path="external/v8" name="platform/external/v8" />
  <project path="external/valgrind" name="platform/external/valgrind" />
  <project path="external/webkit" name="platform/external/webkit" />
  <project path="external/webp" name="platform/external/webp" />
  <project path="external/webrtc" name="platform/external/webrtc" />
  <project path="external/wpa_supplicant_6" name="platform/external/wpa_supplicant_6" />
  <project path="external/wpa_supplicant_8" remote="androvm" name="platform_external_wpa_supplicant_8" revision="androVM-4.1.1_r6.1" />
  <project path="external/xmlwriter" name="platform/external/xmlwriter" />
  <project path="external/yaffs2" name="platform/external/yaffs2" />
  <project path="external/zlib" name="platform/external/zlib" />
  <project path="external/zxing" name="platform/external/zxing" />
  <project path="frameworks/av" remote="androvm" name="platform_frameworks_av" revision="androVM-4.1.1_r6.1" />
  <project path="frameworks/base" remote="androvm" name="platform_frameworks_base" revision="androVM-4.1.1_r6.1" />
  <project path="frameworks/compile/libbcc" name="platform/frameworks/compile/libbcc" />
  <project path="frameworks/compile/linkloader" name="platform/frameworks/compile/linkloader" />
  <project path="frameworks/compile/mclinker" name="platform/frameworks/compile/mclinker" />
  <project path="frameworks/compile/slang" name="platform/frameworks/compile/slang" />
  <project path="frameworks/ex" name="platform/frameworks/ex" />
  <project path="frameworks/mff" name="platform/frameworks/mff" />
  <project path="frameworks/ml" name="platform/frameworks/ml" />
  <project path="frameworks/native" remote="androvm" name="platform_frameworks_native" revision="androVM-4.1.1_r6.1" />
  <project path="frameworks/opt/calendar" name="platform/frameworks/opt/calendar" />
  <project path="frameworks/opt/emoji" name="platform/frameworks/opt/emoji" />
  <project path="frameworks/opt/inputmethodcommon" name="platform/frameworks/opt/inputmethodcommon" />
  <project path="frameworks/opt/mailcommon" name="platform/frameworks/opt/mailcommon" />
  <project path="frameworks/opt/vcard" name="platform/frameworks/opt/vcard" />
  <project path="frameworks/rs" name="platform/frameworks/rs" />
  <project path="frameworks/support" name="platform/frameworks/support" />
  <project path="frameworks/testing" name="platform/frameworks/testing" />
  <project path="frameworks/wilhelm" name="platform/frameworks/wilhelm" />
  <project path="gdk" name="platform/gdk" />
  <project path="hardware/broadcom/wlan" name="platform/hardware/broadcom/wlan" />
  <project path="hardware/invensense" name="platform/hardware/invensense" />
  <project path="hardware/libhardware" remote="androvm" name="platform_hardware_libhardware" revision="androVM-4.1.1_r6.1" />
  <project path="hardware/libhardware_legacy" name="platform/hardware/libhardware_legacy" />
  <project path="hardware/msm7k" name="platform/hardware/msm7k" />
  <project path="hardware/qcom/gps" name="platform/hardware/qcom/gps" />
  <project path="hardware/qcom/media" name="platform/hardware/qcom/media" />
  <project path="hardware/ril" name="platform/hardware/ril" />
  <project path="hardware/ti/omap3" name="platform/hardware/ti/omap3" />
  <project path="hardware/ti/omap4xxx" name="platform/hardware/ti/omap4xxx" />
  <project path="hardware/ti/wlan" name="platform/hardware/ti/wlan" />
  <project path="hardware/ti/wpan" name="platform/hardware/ti/wpan" />
  <project path="libcore" name="platform/libcore" />
  <project path="libnativehelper" remote="androvm" name="platform_libnativehelper" revision="androVM-4.1.1_r6.1" />
  <project path="ndk" name="platform/ndk" />
  <project path="packages/apps/BasicSmsReceiver" name="platform/packages/apps/BasicSmsReceiver" />
  <project path="packages/apps/Bluetooth" name="platform/packages/apps/Bluetooth" />
  <project path="packages/apps/Browser" name="platform/packages/apps/Browser" />
  <project path="packages/apps/Calculator" name="platform/packages/apps/Calculator" />
  <project path="packages/apps/Calendar" name="platform/packages/apps/Calendar" />
  <project path="packages/apps/Camera" name="platform/packages/apps/Camera" />
  <project path="packages/apps/CellBroadcastReceiver" name="platform/packages/apps/CellBroadcastReceiver" />
  <project path="packages/apps/CertInstaller" name="platform/packages/apps/CertInstaller" />
  <project path="packages/apps/Contacts" name="platform/packages/apps/Contacts" />
  <project path="packages/apps/DeskClock" name="platform/packages/apps/DeskClock" />
  <project path="packages/apps/Email" name="platform/packages/apps/Email" />
  <project path="packages/apps/Exchange" name="platform/packages/apps/Exchange" />
  <project path="packages/apps/Gallery" name="platform/packages/apps/Gallery" />
  <project path="packages/apps/Gallery2" name="platform/packages/apps/Gallery2" />
  <project path="packages/apps/HTMLViewer" name="platform/packages/apps/HTMLViewer" />
  <project path="packages/apps/KeyChain" name="platform/packages/apps/KeyChain" />
  <project path="packages/apps/Launcher2" name="platform/packages/apps/Launcher2" />
  <project path="packages/apps/LegacyCamera" name="platform/packages/apps/LegacyCamera" />
  <project path="packages/apps/Mms" name="platform/packages/apps/Mms" />
  <project path="packages/apps/Music" name="platform/packages/apps/Music" />
  <project path="packages/apps/MusicFX" name="platform/packages/apps/MusicFX" />
  <project path="packages/apps/Nfc" name="platform/packages/apps/Nfc" />
  <project path="packages/apps/PackageInstaller" name="platform/packages/apps/PackageInstaller" />
  <project path="packages/apps/Phone" name="platform/packages/apps/Phone" />
  <project path="packages/apps/Protips" name="platform/packages/apps/Protips" />
  <project path="packages/apps/Provision" name="platform/packages/apps/Provision" />
  <project path="packages/apps/QuickSearchBox" name="platform/packages/apps/QuickSearchBox" />
  <project path="packages/apps/Settings" remote="androvm" name="platform_packages_apps_Settings" revision="androVM-4.1.1_r6.1" />
  <project path="packages/apps/SoundRecorder" name="platform/packages/apps/SoundRecorder" />
  <project path="packages/apps/SpareParts" name="platform/packages/apps/SpareParts" />
  <project path="packages/apps/SpeechRecorder" name="platform/packages/apps/SpeechRecorder" />
  <project path="packages/apps/Stk" name="platform/packages/apps/Stk" />
  <project path="packages/apps/Tag" name="platform/packages/apps/Tag" />
  <project path="packages/apps/VideoEditor" name="platform/packages/apps/VideoEditor" />
  <project path="packages/apps/VoiceDialer" name="platform/packages/apps/VoiceDialer" />
  <project path="packages/experimental" name="platform/packages/experimental" />
  <project path="packages/inputmethods/LatinIME" name="platform/packages/inputmethods/LatinIME" />
  <project path="packages/inputmethods/OpenWnn" name="platform/packages/inputmethods/OpenWnn" />
  <project path="packages/inputmethods/PinyinIME" name="platform/packages/inputmethods/PinyinIME" />
  <project path="packages/providers/ApplicationsProvider" name="platform/packages/providers/ApplicationsProvider" />
  <project path="packages/providers/CalendarProvider" name="platform/packages/providers/CalendarProvider" />
  <project path="packages/providers/ContactsProvider" name="platform/packages/providers/ContactsProvider" />
  <project path="packages/providers/DownloadProvider" name="platform/packages/providers/DownloadProvider" />
  <project path="packages/providers/DrmProvider" name="platform/packages/providers/DrmProvider" />
  <project path="packages/providers/MediaProvider" name="platform/packages/providers/MediaProvider" />
  <project path="packages/providers/PartnerBookmarksProvider" name="platform/packages/providers/PartnerBookmarksProvider" />
  <project path="packages/providers/TelephonyProvider" name="platform/packages/providers/TelephonyProvider" />
  <project path="packages/providers/UserDictionaryProvider" name="platform/packages/providers/UserDictionaryProvider" />
  <project path="packages/wallpapers/Basic" name="platform/packages/wallpapers/Basic" />
  <project path="packages/wallpapers/Galaxy4" name="platform/packages/wallpapers/Galaxy4" />
  <project path="packages/wallpapers/HoloSpiral" name="platform/packages/wallpapers/HoloSpiral" />
  <project path="packages/wallpapers/LivePicker" name="platform/packages/wallpapers/LivePicker" />
  <project path="packages/wallpapers/MagicSmoke" name="platform/packages/wallpapers/MagicSmoke" />
  <project path="packages/wallpapers/MusicVisualization" name="platform/packages/wallpapers/MusicVisualization" />
  <project path="packages/wallpapers/NoiseField" name="platform/packages/wallpapers/NoiseField" />
  <project path="packages/wallpapers/PhaseBeam" name="platform/packages/wallpapers/PhaseBeam" />
  <project path="pdk" name="platform/pdk" />
  <project path="prebuilt" name="platform/prebuilt" />
  <project path="prebuilts/eclipse" name="platform/prebuilts/eclipse" />
  <project path="prebuilts/gcc/darwin-x86/arm/arm-eabi-4.6" name="platform/prebuilts/gcc/darwin-x86/arm/arm-eabi-4.6" />
  <project path="prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.6" name="platform/prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.6" />
  <project path="prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.4.3" name="platform/prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.4.3" />
  <project path="prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.6" name="platform/prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.6" />
  <project path="prebuilts/gcc/darwin-x86/x86/i686-android-linux-4.4.3" name="platform/prebuilts/gcc/darwin-x86/x86/i686-android-linux-4.4.3" />
  <project path="prebuilts/gcc/darwin-x86/x86/i686-linux-android-4.6" name="platform/prebuilts/gcc/darwin-x86/x86/i686-linux-android-4.6" />
  <project path="prebuilts/gcc/linux-x86/arm/arm-eabi-4.6" name="platform/prebuilts/gcc/linux-x86/arm/arm-eabi-4.6" />
  <project path="prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.6" name="platform/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.6" />
  <project path="prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.4.3" name="platform/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.4.3" />
  <project path="prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.6" name="platform/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.6" />
  <project path="prebuilts/gcc/linux-x86/host/x86_64-linux-glibc2.7-4.6" name="platform/prebuilts/gcc/linux-x86/host/x86_64-linux-glibc2.7-4.6" />
  <project path="prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.4.3" name="platform/prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.4.3" />
  <project path="prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.6" name="platform/prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.6" />
  <project path="prebuilts/gcc/linux-x86/x86/i686-android-linux-4.4.3" name="platform/prebuilts/gcc/linux-x86/x86/i686-android-linux-4.4.3" />
  <project path="prebuilts/gcc/linux-x86/x86/i686-linux-android-4.6" name="platform/prebuilts/gcc/linux-x86/x86/i686-linux-android-4.6" />
  <project path="prebuilts/misc" name="platform/prebuilts/misc" />
  <project path="prebuilts/ndk" name="platform/prebuilts/ndk" />
  <project path="prebuilts/qemu-kernel" name="platform/prebuilts/qemu-kernel" />
  <project path="prebuilts/sdk" name="platform/prebuilts/sdk" />
  <project path="prebuilts/tools" name="platform/prebuilts/tools" />
  <project path="sdk" remote="androvm" name="platform_sdk" revision="androVM-4.1.1_r6.1" />
  <project path="system/bluetooth" name="platform/system/bluetooth" />
  <project path="system/core" remote="androvm" name="platform_system_core" revision="androVM-4.1.1_r6.1" />
  <project path="system/extras" name="platform/system/extras" />
  <project path="system/media" name="platform/system/media" />
  <project path="system/netd" name="platform/system/netd" />
  <project path="system/security" name="platform/system/security" />
  <project path="system/vold" remote="androvm" name="platform_system_vold" revision="androVM-4.1.1_r6.1" />

  <project path="device/androVM" remote="androvm" name="device_androVM" revision="androVM-4.1.1_r6.1" />
  <project path="external/busybox" remote="androvm" name="platform_external_busybox" revision="androVM-4.1.1_r6.1" />
  <project path="packages/apps/Superuser" remote="androvm" name="platform_packages_apps_Superuser" revision="androVM-4.1.1_r6.1" />

</manifest>
