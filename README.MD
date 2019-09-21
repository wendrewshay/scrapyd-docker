# scrapyd-docker镜像构建

### 实践系统：centos7，python版本：3.7
* 在centos7目录下cd到compile文件夹编译docker镜像：docker build -t scrapyd:latest . ，将镜像上传到公共或私有仓库
* cd到docker-compose.yml所在目录下，运行镜像实例：docker-compose up -d