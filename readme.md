请不要fork！！！fork太多会导致项目直接挂掉,如需使用，请在右上角选择新建项目，导入代码
## 使用注意 :warning:

- :warning: 请不要fork，因为GitHub Actions也会fork过去。那样会给番组计划的服务器造成压力；又或者请求过多，有可能触发拒绝请求的保护机制，造成项目被后台删除。

- :warning: lxk大佬的代码已私人化，请自寻路径了，以前的代码不更新还能用


  详细的教程在wiki> https://gitee.com/wudongdefeng/jd-base/wikis <

  依次按下顺序运行代码  

  mkdir ~/.ssh

  lxk大佬的密钥复制到~/.ssh  

  使用termux高级教程配置好，百度第一个就是  

  pkg update  

  pkg install git perl nodejs-lts wget curl nano cronie moreutils  

  git clone https://gitee.com/wudongdefeng/jd-base.git ~/storage/shared/jd  

  cd  ~/storage/shared/jd  

  cp sample/auth.json config/auth.json  

  cp sample/termux.list.sample config/crontab.list  

  cp ~/storage/shared/jd/sample/config.sh.sample config/config.sh  

  bash git_pull.sh  

  至此代码已OK！  

  控制面板开启方法  

  cd panel  

  npm install || npm install --registry=https://registry.npm.taobao.org.com  

  node server.js  

 出现端口5678提示，进手机网页127.0.0.1:5678就好了（当然用pm2也行，但是用pm2不容易发现错误，会导致控制面板能显示但为空白，建议node server.js成功后再使用pm2) 
  

 出现错误无非是npm的问题，自己在网页搜索相关的教程，一般重新安装nodejs-lts就能解决  

 最后代码怎么运行呢  

 crond ~/storage/shared/jd/config/crontab.list
  
 crond
 
 好了代码已全自动了，切记每次重启软件需要重新运行这句上面两行代码。
  

 
 


