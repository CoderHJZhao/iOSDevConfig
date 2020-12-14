# iOSDevConfig
iOS开发环境配置

homebrew环境配置（国内镜像，清华大学的会快一些）
/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"
如果遇到以下错误：
Cloning into '/usr/local/Homebrew'...
remote: Counting objects: 164925, done.
remote: Compressing objects: 100% (43110/43110), done.
fatal: the remote end hung up unexpectedly.75 MiB | 120.00 KiB/s
fatal: early EOF
fatal: index-pack failed
此步骤失败 尝试再次运行自动脚本选择其他下载源或者切换网络

运行：git config --global http.postBuffer 524288000
然后再运行：
/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"
ruby更新：

更换国内下载源：
删除原有的
gem sources --remove https://rubygems.org/
替换
gem source -a https://gems.ruby-china.com/
查看当前的源地址
gem sources -l
更新
sudo gem update --system

rvm安装，无需配置
brew install rvm

cocoapods安装
sudo gem install -n /usr/local/bin cocoapods
pod setup
