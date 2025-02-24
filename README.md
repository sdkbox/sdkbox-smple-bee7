
# How to run sdkbox samples

Steps:

~~~bash
mkdir samples
cd samples

# must clone this repo
git clone --depth 1 https://github.com/sdkbox/sdkbox-cocos2d-x-binary.git

# clone sample repo
git clone --depth 1 https://github.com/sdkbox/sdkbox-sample-bee7.git

# run sample with specified language and platform
# eg: cpp and ios
./sdkbox-cocos2d-x-binary/run_sample.sh bee7 cpp ios
## or
cd cpp && cocos run -p ios

# javascript and android
./sdkbox-cocos2d-x-binary/run_sample.sh bee7 js android
## or
cd js && cocos run -p android

# <optional> if exists "download-depends.sh" in sample repo, execute it
# ./sdkbox-sample-bee7/download-depends.sh

~~~

Memo:

1.  Sample repo and cocos2dx repo must be in same level directory

~~~
+-- sdkbox-cocos2d-x-binary
+-- sdkbox-sample-bee7
| +-- cpp
| +-- lua
| \-- js
~~~
