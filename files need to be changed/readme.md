
openwrt/package/lean/default-settings/files/zzz-default-settings

https://www.bandwh.com/net/38.html
https://jao.gitbook.io/project/linux/openwrt/compile/lean-4.14
https://3mile.top/archives/2019/0525110729/

固化 /etc/config
（编译保存你的配置）files大法：实际就是把现在的配置以文件的形式固化到新固件里。这样做的好处就是升级不需要保留配置，或者恢复出厂设置，缺省值就是你自己设置好的配置 固化某配置教程例子： 1.提取路由固件下的\etc\config\network 2.在编译机LEDE根目录下创建files目录 3.拷贝到 \files\etc\config\network 这样编译完，network就是你自己配置好的network，注意提取的文件路径和权限要一致

\etc\config                                      各个LUCI配置
\etc\gfwlist                                     gfwlist目录
\etc\shadow                                      登录密码
\etc\firewall.user                               自定义防火墙规则
\usr\share\adbyby                                adbyby里的相关规则和设置
\usr\lib\lua\luci\view\admin_status\index.htm    主页样式文件，温度显示等等
etc/config/system #里面有主机名，时区，ntp时间服务器设置
etc/config/network #网络设置
etc/config/dhcp    #如果对dhcp有分配ip
etc/config/ddns    #ddns设置
etc/config/aliddns #aliddns设置
etc/config/adbyby  #广告过滤大师设置 ，如果有自定义广告过滤大师可以复制过去
etc/config/firewall #防火墙
etc/config/gfw.ilst #自定义gfw列表