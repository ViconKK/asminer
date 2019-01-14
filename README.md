# asminer
agent-server miner

## 下载

* 下载 ：https://github.com/ViconKK/asminer/releases/tag/0.0.1

## 安装运行

* 例如(darwin) ：
```bash

#>tar xzvf miner-darwin-amd64.tar.gz
#>build/miner-darwin-amd64 -h
Usage of build/miner-darwin-amd64:
  -a string
    	salary account // 指定接收奖励的账户，只支持 eth 体系账户
  -d string
    	set ipfs home dir. // 指定 ipfs 的数据目录，找空间最大的目录设置
  -v	show miner version. // 查看版本号

#>build/miner-darwin-amd64 -a 0xf3adb7b7b9c582098cd77fd133eeb296e69ea1ff -d /data/ipfshome
```

windows 和 linux 与示例相同，都是解压缩然后直接运行可执行文件即可.
