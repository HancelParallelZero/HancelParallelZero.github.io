---
layout: post
title:  "How to install Hancel"
date:   2020-02-12 12:06:03 +0100
categories: post update
---

You can install it from the [release section](https://github.com/HancelParallelZero/hancel_android/releases) downloading the last apk.

# Building (optional)

For build a debug version please install Android SDK and Android Tools and follow the next steps:

``` bash
git clone --recursive https://github.com/HancelParallelZero/hancel_android.git
cd hancel_android
./gradlew assembleDebug
```

## Updates

Is possible that the submodules will be updated in the future, for this, please run before:

``` bash
git submodule update --init --recursive
```

## Troubleshooting

For signed versions and possible `api-key` issues please generate your own API keys for the next services and put it in `app/src/main/res/values/api_keys.xml` like this:

```xml
<resources>
    <string name="key_debug" translatable="false">AIzaSyDvdxR50ECGFT600000000000000000000</string>
    <string name="key_prod" translatable="false">AIzaSyA-s1RQ-pzo8FlNOPkrVn1qy0000000000</string>
    <string name="crashlytics" translatable="false">78deae26fe9c8f597807a086900000000000000</string>
</resources>
```


