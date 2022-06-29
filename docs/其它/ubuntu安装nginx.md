### 1.安装gcc g++的依赖库

```shell
sudo apt-get install build-essential
sudo apt-get install libtool
```

### 2.安装pcre依赖库（http://www.pcre.org/）

```shell
sudo apt-get update
sudo apt-get install libpcre3 libpcre3-dev
```

### 3.安装zlib依赖库（http://www.zlib.net）

```shell
sudo apt-get install zlib1g-dev
```

### 4.安装ssl依赖库（16.04默认已经安装了）

```shell
sudo apt-get install openssl
```

### 5.安装nginx

复制代码
#下载最新版本：

```shell
wget http://nginx.org/download/nginx-1.13.6.tar.gz
```

#解压：

```shell
tar -zxvf nginx-1.13.6.tar.gz
```

#进入解压目录：

```shell
cd nginx-1.13.6
```

#配置：

```shell
./configure --prefix=/etc/nginx 
```

#编译：

```shell
make
```

#安装：

```shell
sudo make install

cd /etc/nginx/conf

```
修改nginx.conf
![在这里插入图片描述](https://img-blog.csdnimg.cn/557d98061e034c8f96c843ee9e24d022.png?x-oss-process=image/watermark,type_d3f5lxplbmhlaq,shadow_50,text_q1netibaqnjpz2h0mty2oa==,size_20,color_ffffff,t_70,g_se,x_16)
![在这里插入图片描述](https://img-blog.csdnimg.cn/e1d9e4da96dd4eebb0148888cc695baa.png?x-oss-process=image/watermark,type_d3f5lxplbmhlaq,shadow_50,text_q1netibaqnjpz2h0mty2oa==,size_19,color_ffffff,t_70,g_se,x_16)
创建 conf.d目录

```shell
mkdir conf.d
```

#启动：
sudo /etc/nginx/sbin/nginx -c /etc/nginx/conf/nginx.conf
注意：-c 指定配置文件的路径，不加的话，nginx会自动加载默认路径的配置文件，可以通过-h查看帮助命令。
#查看进程：

```shell
ps -ef | grep nginx
```

复制代码
配置软链接

```shell
sudo ln -s /etc/nginx/sbin/nginx /usr/bin/nginx
```

这样你就可以在conf.d下面写你的配置文件了

![在这里插入图片描述](https://img-blog.csdnimg.cn/befbb992a3f24c89a41c11b5d3b0dd0e.png)