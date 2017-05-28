yololib
=======

dylib injector for mach-o binaries


Usage
============

#### 1. First of all, using `iOSOpenDev` template to create a project which called `hook`, and write the hook code, then build it to a `hook.dylib`

#### 2. Second of all, using command `command + B` to build `yololib` as an executable binary file, and in the terminal , input the following command 
>./yololib yourAppName.app/yourAppName hook.dylib 

The output message in the Terminal as below:
```
2017-05-28 13:13:22.001 yololib[1079:122842] dylib path @executable_path/hook.dylib
2017-05-28 13:13:22.002 yololib[1079:122842] dylib path @executable_path/hook.dylib
Reading binary: com.tencent.xin-iOS7.0-(Clutch-2.0.4)/Payload/WeChat.app/WeChat

2017-05-28 13:13:22.003 yololib[1079:122842] FAT binary!
2017-05-28 13:13:22.003 yololib[1079:122842] Injecting to arch 9
2017-05-28 13:13:22.003 yololib[1079:122842] Patching mach_header..
2017-05-28 13:13:22.003 yololib[1079:122842] Attaching dylib..

2017-05-28 13:13:22.003 yololib[1079:122842] Injecting to arch 0
2017-05-28 13:13:22.003 yololib[1079:122842] 64bit arch wow
2017-05-28 13:13:22.003 yololib[1079:122842] dylib size wow 56
2017-05-28 13:13:22.003 yololib[1079:122842] mach.ncmds 77
2017-05-28 13:13:22.003 yololib[1079:122842] mach.ncmds 78
2017-05-28 13:13:22.003 yololib[1079:122842] Patching mach_header..
2017-05-28 13:13:22.004 yololib[1079:122842] Attaching dylib..

2017-05-28 13:13:22.004 yololib[1079:122842] size 51
2017-05-28 13:13:22.004 yololib[1079:122842] complete!
```
