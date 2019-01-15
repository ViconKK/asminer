# asminer
agent-server miner

## 下载

* 下载 ：https://github.com/ViconKK/asminer/releases/tag/0.0.1

## 安装运行

* darwin ：
```bash

#>tar xzvf miner-darwin-amd64.tar.gz
#>cd build
#>miner-darwin-amd64 -h
Usage of miner-darwin-amd64:
  -a string
    	salary account // 指定接收奖励的账户，只支持 eth 体系账户
  -d string
    	set ipfs home dir. // 指定 ipfs 的数据目录，找空间最大的目录设置
  -v	show miner version. // 查看版本号

#>./miner-darwin-amd64 -a 0xf3adb7b7b9c582098cd77fd133eeb296e69ea1ff -d /data/ipfshome
```

* windows ：

解压缩后，在 cmd 进入矿工程序所在目录

```bash
#>./miner-windows-amd64.exe -a 0xf3adb7b7b9c582098cd77fd133eeb296e69ea1ff -d d:/ipfshome
```

* linux (amd64/arm)

需要先通过 `-setup` 生成启动脚本，然后通过脚本启动矿工

```bash
#>tar xzvf miner-linux-amd64.tar.gz
#>cd build
#>./miner-linux-amd64 -setup -d /data/ipfshome
#>ls -l
-rwxr-xr-x    1 501      20       101824960 Jan 15 15:16 miner-linux-amd64
-rwxr-xr-x    1 root     root           620 Jan 15 15:19 miner-start.sh
-rwxr-xr-x    1 root     root           104 Jan 15 15:18 miner-stop.sh

#>sh miner-start.sh
//当前目录下会生成日志文件
#>tail -f miner.log
```

# 注意

想收到奖励就要尽量保证本地 `ip` 可以被外面访问，路由器需要开启 `upnp` 而且本地要保证关闭防火墙或者对外开放 `tcp 50001` 端口
