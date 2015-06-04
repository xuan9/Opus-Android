# Opus-Android

A build Android NDK script from: http://stackoverflow.com/questions/17869333/makefile-needed-for-compiling-the-opus-codec-for-android

Steps: 

1. Download the opus source files into 'opus' directory. 
  Opus version 1.1 works well: http://downloads.xiph.org/releases/opus/opus-1.1.tar.gz
  For latest version 1.1.1-beta, a build error happens in the next build step.
  
2. Build it using Android 'ndk-build' command:

	ndk-build APP_BUILD_SCRIPT=Android.mk NDK_PROJECT_PATH=build

3. Find the built static library at 'build/obj/local/armeabi/libopus.a'. 
