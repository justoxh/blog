## Mac Install 

### 安装 Mono

安装程序从 [官网](http://www.mono-project.com/download/#download-mac) 地址下载
安装完成后，打开 Terminal 终端，在 Terminal 里输入如下命令：

```bash
/Library/Frameworks/Mono.framework/Versions/<mono version>/bin/mozroots --import --sync 
```
编辑 .bash_profile

```bash
vim ~/.bash_profile

```

追加

```
export MONO_HOME=/Library/Frameworks/Mono.framework/Versions/6.0.0
export PATH=$PATH:$MONO_HOME/bin 
```

启动环境变量

```
source ~/.bash_profile
```

### 安装 Fiddler 

从 [官网](https://www.telerik.com/download/fiddler) 下载压缩包并解压

切换到解压目录下，运行

```bash
sudo mono Fiddler.exe
```

### 一些问题

看提示好像不支持 64 位，因此需要换成

```
sudo mono --arch=32 Fiddler.exe
```

