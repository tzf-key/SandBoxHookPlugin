# SandBoxHookPlugin

demo for inject &amp; hook in sandbox
you can use in va or dr clone etc....
also can use in a root device...

# How to use

- set hook target:  

public final static String targetPkg = "com.trendmicro.speedy";  

- set abi with hook target:  

abiFilters 'armeabi-v7a'. 

copy libsandhook.so from sandhook to assets

- set hook item  

SandHook.addHookClass(ActivityHooker.class);

- check path with target android version:   

jobject loader = load_module("/data/app/com.swift.hookdemo-1/base.apk");
String soNewPath = "/data/data/" + targetPkg + "/lib/libsandhook32.so";

# Ref

Hook: https://github.com/ganyao114/SandHook  

Inject: https://github.com/hluwa/Android-Injector
