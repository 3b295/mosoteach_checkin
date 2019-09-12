# ⚠️ 停止维护了
这个项目太久没更新无法直接使用, 主要是蓝墨云那边的接口有变动. 感兴趣的同学可以尝试自己改改.

# Mosoteach Checkin

## 快速开始
### 配置
通过抓包，填写config.py中 `SimpleConfig`类。
```
class SimpleConfig:
    # 登陆请求的返回JSON中可以找到
    USER_ID = None
    ACCESS_SECRET = None

    # 签到请求的headers中可以找到
    X_MSSVC_ACCESS_ID = None
    X_MSSVC_SEC_TS = None

    # 每次请求的延迟时间范围, 秒
    INTERVAL = (10, 20)

    # 日志的位置
    LOGGING_PATH = "./logging.txt"

    # 经纬度
    # LNG = "100.000000"
    # LAT = "100.000000"
    LNG = None
    LAT = None

    CLAZZ_COURSE_ID = None
```
### 启动
`python main.py simple`


## 如果使用docker
填写config.py总的配置。
- 切换到项目根目录， 运行构筑`docker build -t moso .`

- 启动: `docker run --rm moso simple`

- 如果需要后台运行 `docker run -d --rm simple`

  ​
## 环境依赖

- Java 8， 需要正确配置环境变量

- Python 3




