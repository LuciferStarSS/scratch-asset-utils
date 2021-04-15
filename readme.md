### 素材处理工具使用说明

支持背景、造型、声音、角色等素材的一键导入，并自动生成缩略图、更新索引。

#### 环境说明

- 运行环境 Python 3.x

- 依赖Pillow，shutil，pysocks



#### 使用说明

1. 默认使用本项目自带的素材库，或者配置相关路径参数

2. 执行python scratch2-asset-process.py

3. 将文件拖入窗口，自动添加本素材，素材名默认为文件名

   将文件夹拖入，则自动处理所有文件

#### 素材格式要求

- 背景素材

  jpg格式，建议尺寸480x320

- 造型素材

  png或svg格式

- 声音素材

  wav格式

- 角色素材

  sprite2格式

  ​


### 官网素材库爬虫使用说明

用于爬取scratch2和scratch3官方CDN上的素材库

#### 环境说明

- 运行环境 Python 3.x


- 依赖requests

#### 使用说明

- 爬取scratch2素材库

直接执行python scratch2-asset-crawl.py 即可

- 爬取scratch3素材库

因为国外资源下载太慢，爬虫使用了socks代理，如果没有的话可以自行去掉
将最新的索引文件放到scratch3/json_index文件夹中，执行python scratch3-asset-crawl.py 即可