# Download Android source with patches(local_manifests)

 Refer to http://source.android.com/source/downloading.html
 
 $ repo init -u https://android.googlesource.com/platform/manifest -b master
 
 $ git clone https://github.com/edge2edge/repo_local_manifests .repo/local_manifests
 
 $ repo sync

# Build

 $ . build/envsetup
 
 $ lunch edge2edge-userdebug
 
 $ make

Use -j[n] option on sync & build steps, if build host has a good number of CPU cores.
