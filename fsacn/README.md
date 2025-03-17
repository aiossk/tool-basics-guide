# fscan
### 安装go环境
```
☠️wget https://golang.org/dl/go1.20.linux-amd64.tar.gz
or google下载
☠️sudo tar -C /usr/local -xzf go1.20.linux-amd64.tar.gz
☠️sudo vim /etc/zsh/zshrc
添加
export GOROOT=/usr/local/go
export GOPATH=/datago
export PATH=$PATH:$GOROOT/bin:$GOPATH
export G0111MODULE="no"
export GOPRXY=https://goproxy.cn,direct
export PATH=/usr/local/go/bin:$PATH
☠️ source /etc/zsh/zshrc
☠️ which go               
/usr/local/go/bin/go                                                                                     
☠️ go version             
go version go1.20 linux/amd64
```
### 安装fscan
```
☠️ git clone https://github.com/shadow1ng/fscan.git
☠️ cd fscan
☠️ go build -ldflags="-s -w" -trimpath main.go
go: could not create module cache: mkdir /datago: permission denied
☠️ mkdir -p $HOME/datago
☠️ chmod u+rwx $HOME/datago
☠️ source /etc/zsh/zshrc
☠️ GOPATH=$HOME/datago  go build -x -ldflags="-s -w" -trimpath main.go
☠️ mv /home/kali/fscan/main /home/kali/fscan/fscan  (改名)
☠️ sudo vim /etc/zsh/zshrc  (添加全局调用变量)
export PATH=$PATH:/home/kali/fscan
☠️source /etc/zsh/zshrc 
```
更多
> https://github.com/shadow1ng/fscan

                 
                                                                                                               


