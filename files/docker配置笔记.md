命令字典：

 docker 镜像： ----class

 docker容器 ： ----实例对象

（一）docker 基础命令
启动docker
systemctl start docker


关闭docker
systemctl stop docker

重启docker
systemctl restart docker

查看docker 运行状态 ------如果是在运行中 输入命令后 会看到绿色的active
systemctl status docker

查看docker 版本号信息
docker version

查看docker 详细信息 --------此命令可以查看到docker 中容器运行个数 以及镜像个数等等
docker info

docker --help 

docker ps        ---列出正在运行的容器

docker ps -a  ----显示所有的容器，包括未运行的



docker -v  查看docker版本

docker pull nginx  下载nginx

docker images 打成镜像

docker run -p 8888:80 -d nginx  使用名为nginx的iamge创建容器并以8888的端口启动(此处可以在docker可视化完成)

docker ps -a  列出正在运行的容器

cd xx/build/  

cd ..

docker cp .\build\ 77e334faab1c://usr/share/nginx/html  将build文件夹拷贝至docker容器内
打开localhost:8888/build/ 访问

