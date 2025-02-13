# RUOYI-CLOUD in docker

```bash
export DOCKER_BUILDKIT=0
docker-compose up -d
```
## RuoYi

> Default account: admin/admin123  

## Sentinel
+ Build image  
    ```bash
    export DOCKER_BUILDKIT=0
    docker build -t sentienl:latest -f dockerfile .
    ```  

+ Run image
    ```bash
    docker run -d -it -p 8888:8080 --name sentinel sentienl:latest
    ```  

    > Default account: sentinel/sentinel  

> https://sentinelguard.io/zh-cn/docs/introduction.html  

## Nacos

> No password  

## Monitor

> Default account: ruoyi/123456  

> https://doc.ruoyi.vip/ruoyi-cloud/cloud/monitor.html#%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%BB%8D  


