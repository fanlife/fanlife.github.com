# 返利网前端

> 博客文档中心

- index.html及index.css为手动创建，其他目录及文件由`travis-ci`中脚本创建并提交

- 目前仅有docs目录，由docs仓库push操作触发travis自动构建，生成docs文件夹提交到当前仓库

- 对文档以及后续可能新增的目录，**不在当前仓库进行操作**，新建仓库处理并由`travis-ci`管理部署

- docs仓库自动构建流程：`travis-ci`监听docs仓库push操作，安装依赖并进行构建相关操作，然后clone本仓库(`fanlife.github.io`)，将上一步构建结果复制到`fanlife.github.io`文件夹下并提交
