# iOSDevConfig
iOS开发环境配置

homebrew环境配置（国内镜像）
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

cocoapods安装
sudo gem install -n /usr/local/bin cocoapods
pod setup
