how to sovle wpa_supplicant compiling error
1.first download the Android Open Source Projcet, Let's go with /Android_Source and 
  $ source ./build/envsetup.sh
2.$ cd Android_Source/external/wpa_supplicant_8/wpa_supplicant/
3.$ mm
  many errors
4.$.cd ../openssl/
5.$.mm
6.many errors:
try to find the missing .so library£º
  $find -maxdepth 10 -name <> //get the name
7.$cd Android_Source/
8.$make missing_lib_name
9.$ cp /root/Android_Sourc/prebuilt/ndk/android-ndk-r6/platforms/android-3/arch-arm/usr/lib/* out/target/generic/obj/system/lib
10.$.cd /Android_Sourc/external/openssl/
11.$.mm
12
$ cd Android_Source/external/wpa_supplicant_8/wpa_supplicant/
$ mm
done!
