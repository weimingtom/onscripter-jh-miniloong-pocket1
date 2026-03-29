# onscripter-jh-miniloong-pocket1
[WIP] My ONScripter-jh Miniloong Pocket 1 port

## Original ONScripter-Jh readme
```
ONScripter是一个开源的NScripter脚本解释工具，主要由Ogapee开发维护
原版的Readme请查看Readme.old。

这是一个修改版的ONScripter源码，在GPLv2协议下发布，使用时请遵守。

修改目标：
	提供比原版ONScripter更好的性能，适当增加一些功能
	添加中文支持
	尽可能的兼容原版ONS脚本
	
进度

	SDL2分支提供各种改进并可在SDL2环境编译
	目前Windows、Android、iOS、Linux、Windows Phone平台均编译通过实测可用，其余平台未测试
```

## [WIP] How to Build  
* Modify Makefile, where are gcc and stage_files   
* Run 'make clean && make MIYOO=1'  

## Cross compile gcc toolchain and SDK stage files    
* SDK_usr_tg5040_a133p.tgz
* https://github.com/trimui/toolchain_sdk_smartpro/releases/tag/20231018

## Differences from old version
* onscripter_old is built from https://github.com/weimingtom/onscripter-jh-trimui-smart-pro-s/tree/master/old_sdk_tg5040, but lose jpg if launched from FileManager.  
* If launched from ports, no this bug.
* But this new code of onscripter fixed this bug, doesn't lose jpg if launched from FileManager.
