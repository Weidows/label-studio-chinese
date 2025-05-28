
[English](./README.md) | 简体中文 


问题联系（可接二次开发）：

微信: hujiao0314

哔哩哔哩主页：https://space.bilibili.com/676568590


# labelstudio-chinese
更适合中国宝宝的labelstudio标注平台

# 更新内容
1.进行了内容汉化

2.修改了用户数据隔离

# 项目启动
### 本地运行 
您可以在本地运行最新的Label Studio版本，而无需从pypi安装软件包。
#### 后端启动模式
```bash
# 安装所有包依赖项
pip install poetry
poetry install
# 运行数据库迁移
python label_studio/manage.py migrate
# 执行django命令进行静态文件和html整合
python label_studio/manage.py collectstatic
# 在开发模式下启动服务器http://localhost:8080
python label_studio/manage.py runserver
```

#### 前端开发模式 （可选）
```bash
# 安装所有包依赖项
cd web 
yarn install --frozen-lockfile;
# 主程序页面启动命令
yarn ls:watch
# 项目数据管理页面启动命令
yarn dm:watch
# 标注插件页面启动命令
yarn lsf:watch
```



## 相关项目

| 项目                                                                                                                   | 描述                                                   |
|----------------------------------------------------------------------------------------------------------------------|------------------------------------------------------|
| label-studio                                                                                                         | 服务端页面，作为pip包分发                                       |
| [Frontend library](web/libs/editor/)                                                                                 | Label Studio前端库（前端标注插件）。这使用React构建UI和mobx状态树进行状态管理。. |  
| [Data Manager library](web/libs/datamanager/)                                                                        | 项目数据管理项目，主要用于显示数据集项目以及导出等操作.                         | 
| [label-studio-converter](https://github.com/HumanSignal/label-studio-sdk/tree/master/src/label_studio_sdk/converter) | 数据转换包，主要用于其他数据格式转换成labelstudio格式，回显到labelstudio中     |
| [label-studio-transformers](https://github.com/HumanSignal/label-studio-transformers)                                | Transformers SDK，Transformers 库和labelstudio集成相关的SDK包 |


