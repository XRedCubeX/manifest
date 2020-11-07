LineageOS 0.1  
Local manifest for Meizu M2 (mblu2)
===========================

Getting Started
---------------

Initialize a repository from LineageOS:

	repo init -u git://github.com/LineageOS/android.git -b lineage-17.1
 
Add local manifest and sync:

	mkdir -p .repo/local_manifests
	curl https://raw.githubusercontent.com/XRedCubeX/manifest/lineage-17.1/mblu2.xml -o .repo/local_manifests/mblu2.xml
	repo sync
 
Build the code:

	source build/envsetup.sh
	breakfast mblu2
	mka bacon 2>&1 | tee build.log
