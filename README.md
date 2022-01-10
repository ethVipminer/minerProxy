## MinerProxy
一键搭建抽水中转平台，只支持ETH，版本已稳定 最稳定的ETH以太坊代理中转矿池程序，MinerProxy/矿池代理，支持TCP和SSL协议，支持自定义抽水，高性能高并发，支持web界面管理。
**************************************
## centos下
```bash
yum update    
yum install git
```
## ubuntu下
```bash
sudo apt-get update -y
sudo apt-get install redir -y
```
**************************************
## 继续......
```bash
git clone https://github.com/ethVipminer/minerProxy.git    
cd minerProxy     
chmod -R 777 minerProxy_web    
nohup ./minerProxy_web &    
（*此句 & 一定要带上，两次回车）    
tail -f nohup.out    
```

记住token（忘记目录下命令：cat  config.yml  （可以查看token））

浏览器http://您的ip:18888(或18889)

#粘贴token
..........................
### 要运行多个代理矿池,设置不同的本地端口即可

#填写格式：
```bash
tcp://eth.f2pool.com:6688    
ssl://asia2.ethermine.org:5555
```


### 后台运行时关闭

```bash
killall minerProxy
```
### 后台运行时查看
```bash
tail -f nohup.out
```

## Windows-CMD下
```bash
运行minerProxy_web.exe
打开防火墙的18888端口，在网页上输入你的IP:18888，输入token，即可配置
config.yml  （可以查看token）
```


## 重要说明

推荐使用香港节点,flexpool和ethermine都可以到50ms左右,延迟率在0.5%-0.9%之间
该软件系统占用极小,开最便宜的云服务器即可

