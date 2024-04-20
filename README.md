# Arcaea Forum
## YinMo19

这是一个将会搭建在校园网内网中的小论坛。考虑前后端分离的设计思想，考虑使用`pip`自带的包管理系统。

---
## 任务执行计划
- [ ] [3] 注册页面设计
- [ ] [2] 注册页面api设计，后端实现
- [ ] [2] 前后对接，测试


---
## 启动虚拟环境

```bash
python -m venv venv
source venv/bin/activate
```
虚拟环境已经在`.gitignore`中忽略，请将它放在`backend`下。
## 安装依赖
在命令行中的`backend`文件夹下直接执行
```bash
pip install -r requirements.txt
```
即可安装所有的依赖项。如果需要新添加依赖，以
```
django==5.0.4
```
的格式添加。

---
## 存储服务使用MinIO

```sh
wget https://dl.min.io/server/minio/release/linux-amd64/minio
chmod +x minio
sudo mv minio /usr/local/bin/
```

然后在命令行中输入
```bash
minio serve storage
```
即可。