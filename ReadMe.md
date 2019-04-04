
部署dev步骤：
1. 下载voten-form-htjy项目
git clone https://github.com/316189693/voten-forum-htjy.git

2. 进入到voten-form-htjy目录， 并下载voten-forum-dock-htjy
cd voten-form-htjy
git submodule add -b develop https://github.com/316189693/voten-forum-dock-htjy.git

3. 进入到voten-forum-dock-htjy目录， 安装各个docker 容器：
docker-compose up -d nginx mysql redis workspace elasticsearch laravel-echo-server 



问题： Error starting userland proxy: mkdir /port/tcp:0.0.0.0:6379:tcp:172.22.0.3:6379: input/output error
解决： 重启docker