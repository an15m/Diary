dpkg安装.deb文件,但不会解决模块的依赖关系,且不会关心ubuntu的软件仓库内的软件,可以用于安装本地的deb文件
apt会解决和安装模块的依赖问题,并会咨询软件仓库, 但不会安装本地的deb文件, apt是建立在dpkg之上的软件管理工具
如果在用dpkg安装.deb遇到依赖问题，那就需要通过
apt-get depends package
来查询依赖关系再用dpkg逐个去安装
