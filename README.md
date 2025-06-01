# 开源机器学习算法可视化平台DemoHub

Todo list：
- 图片校验，数据库已有的图片不再重复上传
- 模型输入输出分离，设计合理的输出内容存储路径
- docker gpu 偶尔会宕机，重启docker可恢复


ssl验证
- 配置http访问，不进行https跳转


docker容器启动命令:
sudo docker run -p 443:443 -itd --name demodocker -v /home/user/demohub_data/:/root --gpus all demoimage:v4
 
 - 如遇到docker start demodocker 报gpu错误，可尝试重启docker: sudo systemctl restart docker