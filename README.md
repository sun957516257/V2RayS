# V2RayS
一个V2Ray的Windows客户端

## 说明
本程序的目的是尽量简单的使用V2Ray，虽然在初期做了许多可以修改配置的功能，但是我后来决定将其禁用了。因此，本程序有如下的重点说明：
### 只支持HTTP代理：
虽然可以通过修改配置文件实现使用socks代理等，但还是建议只使用HTTP代理。
### PAC服务：
自带PAC的服务器，程序会自动设置Win系统的代理，可以设置为使用PAC文件以及全部使用代理，因此，请确保程序目录下有pac.txt文件，本程序自带了一个pac文件，也可以使用自己的。
### config.json文件：
config.json文件是V2Ray的配置文件，直接使用V2Ray自带的配置文件可能引起程序出错，因此自带了config.json文件，同时程序只使用Vmess协议，也可以通过修改这个文件实现mKcp、mux等功能，后期计划添加直接通过界面设置的方式。
因为已经使用pac文件做了是否使用代理的判断，因此删除了配置文件路由功能中关于大陆IP地址或网站判断的部分。
### 使用方式：
目前直接解压运行即可，程序会修改注册表实现自动启动、修改IE代理设置等，若有警告请允许。程序退出时会删除已设置的IE代理，但若程序崩溃或直接终止任务，可能会引起IE代理没有还原，请手动修改。

## 本程序运行需要.NET Framework 4.6